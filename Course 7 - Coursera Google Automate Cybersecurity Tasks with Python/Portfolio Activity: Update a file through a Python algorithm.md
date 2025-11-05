# Portfolio Activity: Update a file through a Python algorithm

# Update a File Through a Python Algorithm

## Activity Overview

In this activity, you will create a portfolio document that demonstrates your experience using Python to develop algorithms for opening files and parsing their contents. This document will serve as part of your cybersecurity portfolio, which you can share with prospective employers or recruiters. The exercise builds on the **Create another algorithm** lab that you completed earlier, allowing you to explain and document your code for professional use.

## Scenario

You work as a security professional in a healthcare company. One of your responsibilities involves managing a file that lists employees authorized to access restricted content based on their IP addresses. There is an **allow list** containing permitted IPs and a **remove list** identifying IPs that should be deleted from the allow list.

Your task is to develop a Python algorithm that checks if any IP addresses from the remove list appear in the allow list. If matches exist, the algorithm removes those IPs from the allow list and updates the file accordingly.

This process ensures only authorized employees retain access to the restricted subnetwork and that all access changes are properly documented.

---

## Step-By-Step Instructions

### Step 1: Access the Template
Use the **Algorithm for file updates in Python** template provided.  
If you do not have a Google account, download the file directly from the provided attachment.

Keep the supporting material **Instructions for including Python code** open for reference as you proceed.

---

### Step 2: Open the File That Contains the Allow List
Assign the file name `"allow_list.txt"` to a variable called `import_file`.  
Use a **with statement** and the `open()` function to read the file safely. Store its contents in a variable called `file`.


---

### Step 3: Read the File Contents
Use the `.read()` method to convert the file’s contents into a string, and assign it to a variable called `ip_addresses`.



---

### Step 4: Convert the String into a List
Convert the string of IP addresses into a list using the `.split()` method.



This allows individual IP addresses to be processed and modified.

---

### Step 5: Iterate Through the Remove List
Create a **for loop** to iterate through `remove_list` using `element` as the loop variable.



---

### Step 6: Remove IP Addresses That Are on the Remove List
Inside the loop, use an **if condition** to check if each `element` is in `ip_addresses`.  
If it is, use `.remove()` to delete that IP from the allow list.



---

### Step 7: Update the File With the Revised List of IP Addresses
Once the IPs are removed, use `.join()` to convert the list back into a string separated by newlines.



Then use another **with statement** and the `.write()` method to overwrite the original file with the updated data.

### Step 8: Project Description

This project demonstrates how Python can be used to manage access control through automated file updates. The algorithm reads a list of authorized IPs, compares it to a list of revoked IPs, and removes any revoked entries. It updates the original file with only the approved IPs, ensuring that the data remains accurate and current.

The exercise highlights file handling, string manipulation, and iteration techniques that are vital in cybersecurity automation tasks.

### Step 9: Summary

The algorithm begins by opening the allow_list.txt file and reading its contents. It converts the data into a list to make the IP addresses easier to work with. It then loops through the remove_list, checking for matches and removing any unauthorized IPs. Once the removal process is complete, the updated list is joined into a string and written back to the file. This workflow ensures access lists remain secure and accurate without manual intervention.

### What to Include in Your Response

Screenshots or typed versions of your Python code

Explanations of the syntax, functions, and keywords used

A clear project description and summary

Details about:

with statement and open() function

.read() and .write() methods

.split() and .join() methods

For loop structure

.remove() method

### Step 10: Self-Assessment Checklist

You should confirm that:

All code sections are included or properly described.

Explanations of Python syntax, functions, and keywords are accurate.

A clear project description is written.

A concise summary highlights key parts of the algorithm.

The file opening and writing processes are explained.

The .read() and .split() steps are correctly described.

The for loop and .remove() method logic are clear.

The file update process using .join() and .write() is included.

The final document is professional and ready for portfolio use.

# Algorithm for file updates in Python

## https://docs.google.com/document/d/10ijJytguD8a-AS8PJ9379a7buCCw_4wZQ9cQZLZ3zdk/edit?usp=sharing
