# Activity Overview

In this activity, you will investigate a suspicious email and identify signs of a phishing attack. You will decide whether the message should be allowed or quarantined.

Phishing is a common and dangerous social engineering method used to steal data or install malware. Recognizing phishing indicators helps protect users and improve organizational security.

---

## Scenario

You are a **security analyst** at an investment firm called **Imaginary Bank**.  
An executive received a **spear phishing email** that appears to come from the board of the company. The email asks them to install new collaboration software called **ExecuTalk**.  

The executive suspects something is off because **ExecuTalk** was never discussed in any previous meetings. They forwarded the message to your team for verification. Your task is to investigate and determine whether the email should be **allowed** or **quarantined**.

---

## Step-by-Step Instructions

### Step 1: Analyze the Suspicious Message

Here’s the full email:

From: imaginarybank@gmail.org

Sent: Saturday, December 21, 2019 15:05:05
To: cfo@imaginarybank.com

Subject: RE: You are been added to an ecsecutiv's groups

Conglaturations! You have been added to a collaboration group ‘Execs.’

Downlode ExecuTalk to your computer.

Mac® | Windows® | Android™

You're team needs you! This invitation will expire in 48 hours so act quickly.

Sincerely,
ExecuTalk©
All rights reserved.


### Step 2: Examine the Email Header

Look closely at the **From** and **To** fields, and the **Subject line**:

- From: `imaginarybank@gmail.org`  
- To: `cfo@imaginarybank.com`  
- Subject: “RE: You are been added to an ecsecutiv's groups”

**Clues to identify phishing:**
- The sender uses a **personal domain** (`@gmail.org`) instead of the company domain (`@imaginarybank.com`).  
- The subject and body contain **spelling and grammar errors** (“Conglaturations,” “Downlode,” “ecsecutiv’s”).  
- The message includes **urgency and pressure tactics** (“expires in 48 hours”).  
- It prompts the recipient to **download software**, which is a common malware delivery method.

---

## Step 3: Identify Phishing Indicators

Add notes to your worksheet summarizing signs that the email is malicious:

1. The sender domain is **not official**, indicating spoofing or impersonation.  
2. Multiple **spelling and grammatical mistakes** lower credibility.  
3. The **urgent tone** pushes the recipient to act without verifying.  
4. The **download link** is suspicious and could install malware.  

---

## Step 4: Determine the Appropriate Action

Based on your analysis, classify the email as **phishing** and **quarantine** it.

**Reasoning:**
- The email impersonates a legitimate organization.
- It uses manipulation tactics to encourage unsafe downloads.
- Allowing it could compromise the executive’s workstation and the company’s internal network.

---

## Step 5: Recommend Mitigation Steps

Include the following recommendations in your report:

- **Quarantine and report** the email to the IT security team.  
- **Block** the sender domain and flag similar patterns in future filters.  
- **Alert employees** about this phishing attempt and reinforce awareness training.  
- **Verify software installations** only through approved company channels.

---

## What to Include in Your Response

Your completed activity should include:

- 2–3 sentences identifying suspicious signs in the email.  
- 1–2 sentences explaining why the message is a phishing attempt.  
- A clear statement that the email should be **quarantined**, not allowed.  
- 2–3 recommendations for preventing future phishing incidents.

## Questions and Answers

### 1. Which two clues in the message header indicate this is a phishing attempt?

The subject line appears to be a reply.

There is a misspelling in the subject line.

The sender is using a different domain.

Correct answers:

There is a misspelling in the subject line.

The sender is using a different domain.

### 2. What details make this message appear legitimate?

The brand labeling

The invitation time limit

The download options for major operating systems

Phishing emails often contain links that redirect to malicious sites or trigger malware downloads.

Pro tip: When investigating suspicious emails, hovering your mouse cursor over buttons will reveal the URL they redirect to without having to click them. This is the safest way to check if it will take you to a suspicious domain or if it links to an http:// URL that isn’t secure.

In this case, the message contains three download options. Each of them opens this login form

Provided Image:
[[https://github.com/shahputra67/google-cybersecurity-portfolio/blob/da4a36d3c94304d55c534caae4210b54237ee761/Course%205%20-%20Assets%2C%20Threats%2C%20and%20Vulnerabilities/Suspicious%20Domain.jpg]]

### 3. The download options open a webpage with a login form. What is the main clue that indicates this form is malicious?

The URL

### 4. After completing your investigation, should this email be quarantined?

Yes
