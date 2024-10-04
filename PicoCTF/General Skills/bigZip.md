# Big Zip

- [Challenge information](#challenge-information)
- [Solution](#solution)

## Challenge information
```
Tags: picoGym Exclusive, General Skills, Easy
Author: LT 'SYREAL' JONES

Description:
Unzip this archive and find the flag.

Challenge link: [https://play.picoctf.org/practice/challenge/322]
```
## Solution


```
1. Wget the link to download the files.
2. Unzip the files. In my case, I used the following command:
    7z x big-zip-files.zip
3. List the files in the directory to get an idea of what we are dealing with.
4. Search for the flag using grep. The command I used is:
    grep pico -r ./big-zip-files 
   Reasoning: The flag is usually in the format picoCTF{<flag>}
```
