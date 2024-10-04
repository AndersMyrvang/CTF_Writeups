# First Find

- [Challenge information](#challenge-information)
- [Solution](#solution)

## Challenge information
```
Tags: picoGym Exclusive, General Skills, Easy
Author: LT 'SYREAL' JONES

Description:
Unzip this archive and find the file named 'uber-secret.txt'

Challenge link: [https://play.picoctf.org/practice/challenge/320]
```
## Solution


```
1. Wget the link to download the files.
2. Unzip the files. In my case, I used the following command:
    7z x big-zip-files.zip
3. List the files in the directory to get an idea of what we are dealing with.
4. Go throught the three directories and since you are looking for a file that is not visible with the ls command. Use the following command to list all files in the directory:
    ls -a
5. Find the file named 'uber-secret.txt' and read the contents.
    cat uber-secret.txt
```
