# Understanding Hashing Lab

This lab aims to familiarize you with the hashing process through Linux.

### Update Package List:
Open a terminal and execute: apt-get update

### Install Missing Utilities (e.g., nano):
Execute: apt-get install nano


Boot up your Kali Linux Virtual Machine.
Open Terminal:

### Gain Root Privileges:
Type sudo su and press Enter.

### Create a New Directory:
Execute: mkdir mydirectory

### Change Working Directory:
Execute: cd mydirectory

### Create a File with Specific Text:
Execute: echo 'this is my content' > file1.txt

### Verify File Content:
Execute: cat file1.txt

### Create Three More Files:
Execute:
echo 'this is my second content' > file2.txt
echo 'this is my third content' > file3.txt
echo 'this is my fourth content' > file4.txt

### List Files in the Directory:
Execute: ls
Expected Output: file1.txt file2.txt file3.txt file4.txt

### Calculate MD5 Hash of file1.txt:
Execute: md5sum file1.txt


![image](https://github.com/user-attachments/assets/26d52dc5-21d7-4e11-804a-50efc95112cd)



### Generate MD5 Hash Values for All Text Files:
Execute: md5sum *.txt > checklist.chk

### Display Content of checklist.chk:
Execute: cat checklist.chk


![image](https://github.com/user-attachments/assets/478c1dfb-f1ce-4570-96fd-0f8c538547d4)



### Verify File Integrity:
Execute: md5sum -c checklist.chk
Expected Output: All files are marked as OK.

### Edit file2.txt:
Execute: nano file2.txt
Add a dot ('.') at the end of the content and save changes.


### Verify Changes with MD5 Check:
Execute: md5sum -c checklist.chk


![image](https://github.com/user-attachments/assets/6f075507-c364-4123-9d68-adefc300d22d)



### View New MD5 Value for file2.txt:
Execute: md5sum file2.txt


### Calculate SHA-1 Hash for file2.txt:
Execute: sha1sum file2.txt

### Generate SHA-1 HMAC with "mysecretkey1":
Execute: cat file2.txt | openssl dgst -sha1 -hmac "mysecretkey1"

### Generate SHA-1 HMAC with "mysecretkey2":
Execute: cat file2.txt | openssl dgst -sha1 -hmac "mysecretkey2"


![image](https://github.com/user-attachments/assets/0f8bd494-2087-4417-b164-17a43826fb24)

