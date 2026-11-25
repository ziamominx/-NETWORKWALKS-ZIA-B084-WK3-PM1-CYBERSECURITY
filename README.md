# NETWORKWALKS — Week 3

## Password Cracking with John the Ripper and NETWORKWALKS Tools

**Project:** B084 — Week 3, Project Module 3  
**Completed by:** Zia Momin

This project demonstrates password-security testing in the provided lab environment. The workflow covers extracting a password hash from an encrypted PDF, testing the hash with John the Ripper (JTR) and the Johnny GUI, and repeating the process with NETWORKWALKS' online tools. The recovered password is then used to verify access to the protected PDF.

> Perform password testing only on files and systems you own or are explicitly authorised to test.

\---

## Part 1 — John the Ripper (JTR) and Johnny GUI

### 1\. Install John the Ripper

Download and install John the Ripper for Windows, or use the version available in Kali Linux.

* https://www.openwall.com/john/
* https://distro.ibiblio.org/openwall/projects/john/1.9.0/

**Screenshot 1 — John the Ripper installation**

!\[alt text](/screenshots3/image-1.png)

### 2\. Install Johnny GUI

Install Johnny and configure it to use the John the Ripper executable.

**Screenshot 2 — Johnny GUI installation**

!\[alt text](/screenshots3/image-2.png)

* https://openwall.info/wiki/john/johnny



### 3\. Configure Johnny

Open Johnny's settings and browse to the John the Ripper executable.

**Screenshot 3 — Johnny settings**

!\[alt text](/screenshots3/image-3.png)

**Screenshot 4 — John.exe configured in Johnny**

!\[alt text](/screenshots3/image-4.png)

### 4\. Obtain the lab PDF and extract its hash

Download the password-protected PDF provided for the exercise, then use a PDF hash-extraction tool.

* https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php

**Screenshot 5 — Encrypted PDF for the lab**

!\[alt text](/screenshots3/image-5.png)

**Screenshot 6 — PDF hash extraction**

!\[alt text](/screenshots3/image-6.png)

### 5\. Save and load the hash

Copy the complete extracted hash into a text file (for example, `hash1.txt`). Import the file into Johnny and start an attack.

**Screenshot 7 — Hash loaded in Johnny**

!\[alt text](/screenshots3/image-7.png)

### 6\. Recover and verify the password

When the attack finishes, view the recovered password and use it to open the protected PDF.

**Screenshot 8 — Password recovery and PDF verification**

!\[alt text](/screenshots3/image-8.png)

\---

## Part 2 — NETWORKWALKS Tools

### 1\. Download the encrypted PDF

Download `My Locked PDF1.pdf` from the project task page:

https://networkwalks.com/project-task-lab-password-cracking-with-networkwalks-tools/

### 2\. Generate the PDF hash

Open the NETWORKWALKS Hash Calculator and upload the locked PDF.

* https://networkwalks.com/hash-calculator/

**Screenshot 9 — NETWORKWALKS Hash Calculator**

!\[alt text](/screenshots3/image-9.png)

**Screenshot 10 — PDF uploaded and hash generated**

!\[alt text](/screenshots3/image-10.png)

### 3\. Copy the complete hash

Copy the entire hash, including the `$pdf$` prefix. Check that the value has not been truncated.

**Screenshot 11 — Complete PDF hash**

!\[alt text](/screenshots3/image-11.png)

### 4\. Run the NETWORKWALKS Password Cracker

Open the Password Cracker and submit the extracted hash.

* https://networkwalks.com/password-cracker/

**Screenshot 12 — NETWORKWALKS Password Cracker**

!\[alt text](/screenshots3/image-12.png)

### 5\. Review the cracking result

Wait for the tool to finish. The time required may vary depending on the password's complexity.

**Screenshot 13 — Password-cracking process**

!\[alt text](/screenshots3/image-13.png)

**Screenshot 14 — Cracking result**

!\[alt text](/screenshots3/image-14.png)

### 6\. Verify the recovered password

Enter the recovered password to open the protected PDF.

**Screenshot 15 — Unlocking the PDF**

!\[alt text](/screenshots3/image-15.png)

**Screenshot 16 — Successful PDF access**

!\[alt text](/screenshots3/image-16.png)

\---

## Conclusion

The practical exercises demonstrated how password hashes can be extracted from a protected PDF and tested with JTR/Johnny and NETWORKWALKS tools. Successfully opening the PDF with the recovered password confirmed the result and highlighted the importance of strong passwords and authorised security testing.

