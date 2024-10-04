# Mod 26

## Challenge information
```
Tags: picoCTF 2021, Cryptography, Easy
Author: madStacks

Description
I wonder what this really is... enc ''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])

Challenge link: [https://play.picoctf.org/practice/challenge/104]
```
## Solution

```
1. The challenge is asking for the flag in ROT13.
2. I used the following command to decode the flag:
    echo "cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_uJdSftmh}" | tr 'A-Za-z' 'N-ZA-Mn-za-m'

Rot13 is a simple letter substitution cipher that replaces a letter with the 13th letter after it in the alphabet.
That is, the letter 'a' is replaced with 'n', 'b' with 'o', 'c' with 'p', and so on.
That is why the command above works. tr is translate and 'A-Za-z' 'N-ZA-Mn-za-m' is the mapping of the letters.
```
