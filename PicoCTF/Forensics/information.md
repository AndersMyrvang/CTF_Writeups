# Information

- [Challenge information](#challenge-information)
- [Solution](#solution)

## Challenge information
```
Tags: picoCTF 2021, Forensics, Easy
Author: susie

Description:
Files can always be changed in a secret way. Can you find the flag? cat.jpg
Challenge link: [https://play.picoctf.org/practice/challenge/186]
```
## Solution

```
1. Download the file cat.jpg.
2. Use binwalk to check if there are any hidden files in the image.
    binwalk -e cat.jpg
3. Since there were no hidden files, I used strings to check for any hidden text in the image.
    strings cat.jpg | grep pico
4. With no results from the previous step, I used exiftool to check for any metadata in the image.
    exiftool cat.jpg
5. Saw that the license was what looked like a base64 encoded string. 
    String: cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9
    I decoded it using:
    echo "cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9" | base64 -d
```
