# Bandit Level 14 to 15 Writeup

Author: [Mohil](https://github.com/mohil2003) (Mention your name, GitHub profile)

Problem Page: [bandit14](https://overthewire.org/bandit/bandit14) (Change this link accordingly)

## List of Commands Used
```
ls - list files in a directory
echo - echo command is used to display line of text/string that are passed as Arguements.
nc - netcat is the command used to read and write along the networks on linux
ssh - enables secure connection to a ssh server on a remote machine
sshpass - enables authentication during ssh via single command 
```

## Walkthrough
'''
As given in the problem statement to submit the password to  current level on localhost port 30000.
This led me to read more about telnet and netcat that help me in this process. 
'''

## Password
`BfMYroe26WYalil77FoDi9qh59eK5xNr`

## Bash/Python script to automate the process
```
!/usr/bin/bash
sshpass -p "4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e" ssh bandit14@bandit.labs.overthewire.org -p 2220 " echo "4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e"|nc localhost 3000"
```