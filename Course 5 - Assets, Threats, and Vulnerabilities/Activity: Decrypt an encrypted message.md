# Linux Cryptography Lab – Decrypting Files with Caesar Cipher and OpenSSL

## Activity Overview
In this activity, you will practice basic cryptographic operations in a Linux environment. You will use encryption and decryption tools to recover hidden messages from encrypted files. This exercise reinforces the importance of cryptography in securing information and teaches how symmetric encryption methods like AES and ciphers like Caesar work in real-world contexts.

---

## Scenario
You are a security analyst working in a Linux environment. All files in your home directory have been encrypted. Your task is to decrypt them by breaking a Caesar cipher and using the OpenSSL command-line tool.  

You will explore your home directory, locate a hidden file, decrypt its message, and then use that message to recover an encrypted data file.

**Current directory:** `/home/analyst`  
**User:** `analyst`

---

## Step-by-Step Instructions

### Task 1: Read the contents of a file
1. Use the `ls` command to list files in your home directory.  
ls
You will see:
Q1.encrypted README.txt caesar
2. Display the contents of the `README.txt` file to read the instructions.  
cat README.txt
The message explains that the `caesar` subdirectory contains a hidden file you need to find and decrypt.

**Check progress:** Completed after reading the file.

---

### Task 2: Find a hidden file
1. Move into the `caesar` subdirectory.  
cd caesar
2. List all files, including hidden ones.  
ls -a

Output:
. .. .leftShift3

Hidden files in Linux begin with a dot (`.`).

3. Display the contents of the hidden file.  

cat .leftShift3

The output is encrypted using a Caesar cipher with a left shift of 3.

4. Decrypt the file using the `tr` command.  


cat .leftShift3 | tr "d-za-cD-ZA-C" "a-zA-Z"

This command translates each letter back by 3 positions in the alphabet. The output reveals the command needed to decrypt the next file.

5. Return to your home directory.  

cd ~

**Check progress:** Completed after decrypting the hidden file.

---

### Task 3: Decrypt a file
1. Use the revealed command to decrypt the main encrypted file.  
openssl aes-256-cbc -pbkdf2 -a -d -in Q1.encrypted -out Q1.recovered -k ettubrute

- **openssl**: Runs the OpenSSL tool  
- **aes-256-cbc**: Uses the AES-256 symmetric encryption algorithm  
- **-pbkdf2**: Adds secure key derivation  
- **-a**: Specifies Base64 encoding  
- **-d**: Decrypts the file  
- **-in**: Specifies the input file  
- **-out**: Specifies the output file  
- **-k**: Provides the decryption password (in this case, `ettubrute`)

2. List the files in your directory again.  


ls

You will now see:


Q1.encrypted Q1.recovered README.txt caesar


3. Display the decrypted message.  
cat Q1.recovered


**Check progress:** Completed after confirming the message is readable.

---

## Conclusion
You have successfully:
- Listed and read files in a Linux directory  
- Found and decrypted a hidden file using a Caesar cipher  
- Decrypted an encrypted file using the OpenSSL AES-256-CBC algorithm  

This lab demonstrates practical command-line cryptography skills essential for understanding data protection, encryption standards, and basic incident recovery processes.

