Update Package List:
Open a terminal and execute: apt-get update

Install Missing Utilities (e.g., nano):
Execute: apt-get install nano


Boot up your Kali Linux Virtual Machine.
Open Terminal:

Gain Root Privileges:
Type sudo su and press Enter.

### Create a New Directory:
Execute: mkdir mydirectory

**Change Working Directory:**
Execute: cd mydirectory

Create a File with Specific Text:
Execute: echo 'this is my content' > file1.txt

Verify File Content:
Execute: cat file1.txt

Create Three More Files:
Execute:
echo 'this is my second content' > file2.txt
echo 'this is my third content' > file3.txt
echo 'this is my fourth content' > file4.txt

List Files in the Directory:
Execute: ls
Expected Output: file1.txt file2.txt file3.txt file4.txt

Calculate MD5 Hash of file1.txt:
Execute: md5sum file1.txt


SCREENSHOT SHOWING MD5 HASH OF FILE1


Generate MD5 Hash Values for All Text Files:

Execute: md5sum *.txt > checklist.chk

Display Content of checklist.chk:
Execute: cat checklist.chk


SCREENSHOT SHOWING MD5 HASH VALUE ALL FILES


Verify File Integrity:
Execute: md5sum -c checklist.chk
Expected Output: All files are marked as OK.

Edit file2.txt:
Execute: nano file2.txt
Add a dot ('.') at the end of the content and save changes.


Verify Changes with MD5 Check:
Execute: md5sum -c checklist.chk


SCREENSHOT SHOWING FILE2 FAILING HASH CHECK


View New MD5 Value for file2.txt:
Execute: md5sum file2.txt


Calculate SHA-1 Hash for file2.txt:
Execute: sha1sum file2.txt

Generate SHA-1 HMAC with "mysecretkey1":
Execute: cat file2.txt | openssl dgst -sha1 -hmac "mysecretkey1"

Generate SHA-1 HMAC with "mysecretkey2":
Execute: cat file2.txt | openssl dgst -sha1 -hmac "mysecretkey2"
