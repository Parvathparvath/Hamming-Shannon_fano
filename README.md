# Huffman-Shannon_fano
# Aim:
Consider a discrete memoryless source with symbols and statistics {0.4, 0.2, 0.2, 0.1, 0.1, } for its output. 
Apply the Huffman and Shannon-Fano to this source. 
Show that by drawing the tree diagram, and 
Calculate the average code word length, entropy, variance, redundancy, and efficiency.
# Tools Required:
# Program:
```
 import math
p = [0.4, 0.2, 0.2, 0.1, 0.1]
lk = [2, 2, 2, 3, 3]
n = len(p)
L = sum(p[k] * lk[k]
for k in range(n))
hs = sum(p[k] * math.log(1 / p[k], 2)
 for k in range(n))
hs = round(hs, 3)
eff = round(hs / L, 3)
red = round(1 - eff, 3)
var = sum(p[k] * (lk[k] - L) ** 2
for k in range(n))
var = round(var, 3)
print(f"Average Codeword Length is : {L}")
print(f"Entropy is : {hs}")
print(f"Efficiency is : {eff * 100}%")
print(f"Redundancy is : {red}")
print(f"Variance is : {var}")
```
# Calculation:
Compare ![WhatsApp Image 2025-09-20 at 15 31 44_858d8bc5](https://github.com/user-attachments/assets/f6bde51b-d1f8-4f28-a645-2ce4479bf9a6)
the manually calculated value and the observed practical value.
# Output

<img width="1682" height="604" alt="Screenshot 2025-09-20 153459" src="https://github.com/user-attachments/assets/418a7a55-06be-4ff6-8d60-3f8a5bf687f7" />
Write the concthlusion
Thus  the average code word length, entropy, variance, redundancy, and efficiency is verified.
