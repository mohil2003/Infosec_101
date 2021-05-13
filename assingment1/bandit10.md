# Bandit Level 10 to 11 Writeup

Author: [Mohil](https://github.com/mohil2003) (Mention your name, GitHub profile)

Problem Page: [bandit10](https://overthewire.org/bandit/bandit10)

## List of Commands Used
```
ls - list files in a directory
base64 - Base64 is a group of binary_to_text encoding schemes that represents binary data in an ASCII string format by translating the data into a radix-64 representation.
echo - echo command is used to display line of text/string that are passed as Arguements.
ssh - enables secure connection to a ssh server on a remote machine
sshpass - enables authentication during ssh via single command 
```

## Walkthrough
'''
I found that the given data.txt file is encoded in base64 format then I went through decoding it and get the password.
'''

## Password
`The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR`

## Bash/Python script to automate the process
```
#!/usr/bin/bash
sshpass -p "truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk" ssh bandit10@bandit.labs.overthewire.org -p 2220 cat data.txt|base64
--decode
```