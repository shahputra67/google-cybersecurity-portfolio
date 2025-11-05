# Activity: Security Incident Investigation

## Activity Overview

In this activity, you will act as a cybersecurity analyst for **YummyRecipesForMe.com**, a website that sells recipes and cookbooks. Visitors to the site experience a security issue when loading the main webpage. Your task is to **investigate, identify, document, and recommend** a solution to the security problem.

You will review a **tcpdump log** to identify the network protocols used between the user and the website. Understanding these protocols helps you recognize how malicious actors exploit them during attacks. You will then document the incident and suggest one security measure to prevent similar attacks in the future.

---

## Scenario

A former employee has executed a **brute force attack** to gain access to the company’s web host. They used several known default passwords until successfully guessing the correct one for the administrative account. After logging in, the hacker:

- Embedded malicious **JavaScript** code in the website’s source code.
- Added a function prompting visitors to download and run a file.
- Changed the admin password to lock out the owner.
- Redirected users to a fake website, **greatrecipesforme.com**, that contained malware.

Several customers emailed the helpdesk claiming they were prompted to download a file to access “free recipes.” After running the file, they noticed their computers slowed down and the website address changed.

When the website owner tried to log in to the admin panel, they were locked out and contacted the hosting provider. The cybersecurity team, including you, was tasked with investigating the issue.

In a **sandbox environment**, you observed the following using tcpdump:

1. The browser initiates a **DNS request** for *yummyrecipesforme.com*.
2. The **DNS server replies** with the correct IP address.
3. The browser sends an **HTTP request** to load the webpage.
4. The browser downloads the malicious file.
5. The browser then makes a **DNS request** for *greatrecipesforme.com*.
6. The **DNS server replies** with that IP address.
7. The browser sends another **HTTP request** to *greatrecipesforme.com*.

A senior analyst confirms that malicious **JavaScript** was added to the source code, redirecting visitors after file execution. The web server was compromised because the **default password** was never changed and **no brute force protection** was in place.

Your task is to **document the incident**, identify the **network protocols involved**, and recommend **one security measure** to prevent brute force attacks.

---

## Step-by-Step Instructions

### Step 1: Access the Template
- Open the **Security Incident Report Template** using the provided link and click **Use Template**.  
- If you don’t have a Google account, download the template directly from the provided attachment.

### Step 2: Access Supporting Materials
Use the supporting materials to complete the activity:
- **tcpdump traffic log**
- **How to Read the tcpdump Log**

If you don’t have a Google account, download these files directly from the provided attachments.

---

### Step 3: Identify the Network Protocol Involved
Use the tcpdump log to determine which **network protocol** appears in the packet captures during the investigation.  
Use your knowledge of the **TCP/IP model** to identify which layer each protocol operates in.

Record the identified protocol in **Section 1** of the Security Incident Report Template.

---

### Step 4: Document the Incident
In **Section 2** of the report, summarize the incident clearly and accurately.

Include:
- Where the incident occurred and how it happened.  
- How it was discovered and by whom.  
- Evidence sources and details of what was affected.  
- Objective, factual information only.

Avoid emotional language (e.g., “terrible,” “awful”).  
Thorough documentation helps other analysts, supports audits, and strengthens security education.

---

### Step 5: Recommend One Remediation for Brute Force Attacks
After documenting the event, choose **one** security measure that would prevent brute force attacks.  
Provide your recommendation in **Section 3** of the template.

Possible options:
- Require **strong passwords**
- Enforce **two-factor authentication (2FA)**
- **Monitor login attempts**
- Require **frequent password changes**
- **Disallow old passwords**
- **Limit login attempts**

Explain why your chosen method is effective in reducing brute force risks.

---

## What to Include in Your Response
Your final submission must include:

- One **network protocol** identified during the investigation  
- A **complete documentation** of the incident  
- One **security measure recommendation** to prevent brute force attacks

# tcpdump traffic log
## https://docs.google.com/document/d/1HDAQTLSK5CyPLPHeLI0s75kNE-kA2kG0NFJoZlz0xCc/template/preview?resourcekey=0-vDSHnW4qKxOOQtsZeGRUeQ

# How to read the tcpdump log 
## https://docs.google.com/document/d/1zuVm_KixJqoHxrMefsxG0bi1tB6RYBQsXkPHIWxdRag/template/preview#heading=h.shz1bcdh2tm3

# Security report incident
## **https://docs.google.com/document/d/1xkrEJHFjxLnqWzFL-AnCaGFVTYPOodYJEspyEyMU2Vo/edit?usp=sharing**
