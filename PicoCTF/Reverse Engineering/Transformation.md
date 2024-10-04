# Transformation

## Challenge information
```
Tags: picoCTF 2021, Reverse Engineering, Easy
Author: madStacks

Description
I wonder what this really is... enc ''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])

Challenge link: [https://play.picoctf.org/practice/challenge/104]
```
## Solution

```
1. Dowload the file enc
2. Decode the encoded message provided in the file:
    灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸彥㜰㍢㐸㙽
3. I used Cyberchef with the encode UTF-16 as recipe and input 灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸彥㜰㍢㐸㙽
```
