# Hashing Files in Linux – Verifying Data Integrity

## Activity Overview
As a security analyst, your role includes protecting organizations from file tampering and integrity issues.  
This activity demonstrates how hashing helps detect unauthorized file changes.  
A **hash function** generates a unique, irreversible code (hash value or digest) for data. If even one character in a file changes, its hash value changes too, allowing you to detect differences.

In this lab, you will generate and compare hash values of two files to determine if they are identical.

---

## Scenario
You are investigating whether two files in your home directory are identical or different.  
Both files appear the same at first glance, but you will use **Linux commands** to verify their integrity by comparing their SHA-256 hashes.

**Goal:** Generate hash values for two files and manually compare them.

**Current directory:** `/home/analyst`  
**Files available:** `file1.txt` and `file2.txt`  
**User:** `analyst`

---

## Step-by-Step Instructions

### Task 1: Generate hashes for files
1. List all files in the home directory:
ls

lua
Copy code
Expected output:
file1.txt file2.txt

markdown
Copy code
2. Display the contents of `file1.txt`:
cat file1.txt

markdown
Copy code
3. Display the contents of `file2.txt`:
cat file2.txt

sql
Copy code
Both files appear identical when viewed with `cat`.

4. Generate SHA-256 hash values for each file:
sha256sum file1.txt
sha256sum file2.txt

lua
Copy code
Example output:
131f95c51cc819465fa1797f6ccacf9d494aaaff46fa3eac73ae63ffbdfd8267 file1.txt
2558ba9a4cad1e69804ce03aa2a029526179a91a5e38cb723320e83af9ca017b file2.txt

yaml
Copy code
The hashes differ, meaning the files are not identical even though they look the same.

**Check progress:** Completed after confirming the hashes differ.

---

### Task 2: Compare hashes
1. Write the hash of `file1.txt` to a new file called `file1hash`:
sha256sum file1.txt >> file1hash

pgsql
Copy code
2. Write the hash of `file2.txt` to a new file called `file2hash`:
sha256sum file2.txt >> file2hash

sql
Copy code
You now have two new files containing the hash values of each text file.

3. Display both hash files to inspect them manually:
cat file1hash
cat file2hash

vbnet
Copy code
The hash values will differ, confirming a file difference.

4. Compare the two hash files byte by byte:
cmp file1hash file2hash

lua
Copy code
Example output:
file1hash file2hash differ: char 1, line 1

The output shows that the hash values differ starting from the first character.

**Conclusion of comparison:**  
`file1.txt` and `file2.txt` are different based on their unique hash values.

**Check progress:** Completed after confirming the difference with `cmp`.

---

## Conclusion
You successfully practiced how to:
- Generate hashes using `sha256sum`  
- Display hash values with `cat`  
- Compare hash files using `cmp`

Hashing ensures **data integrity** by detecting file modifications, a key part of maintaining strong security controls within any organization.
