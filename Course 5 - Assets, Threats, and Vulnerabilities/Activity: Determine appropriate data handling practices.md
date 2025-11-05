# Data Leak Analysis and Least Privilege Review

## Activity Overview
In this activity, you will review the results of a data risk assessment. You will determine whether effective data handling processes are being implemented to protect information privacy.

Data is among the most valuable assets in the world today. Everything from intellectual property to guest WiFi networks should be protected with a combination of technical, operational, and managerial controls. Implementing the principle of least privilege is essential to protect information privacy.

## Scenario
You work for an educational technology company that developed an application to help teachers automatically grade assignments. The application handles a wide range of data that it collects from academic institutions, instructors, parents, and students.

Your team was alerted to a data leak of internal business plans on social media. An investigation discovered that an employee accidentally shared confidential documents with an external business partner. An audit is underway to determine how similar incidents can be avoided.

A supervisor provided you with the details:  
A customer success representative received access to a folder of internal documents from a manager. It contained files related to a new product offering, including customer analytics and marketing materials. The manager forgot to unshare the folder. Later, the representative copied a link to the marketing materials to share with a business partner but mistakenly shared a link to the entire folder. During the sales call, the business partner received the link and posted it publicly on social media.

---

## Step-by-Step Instructions

### Step 1: Access the Template
Use the provided template link and select **Use Template**.  
If you don’t have a Google account, download the template directly from the attachment.

**Template Link:**  
[Data leak worksheet](#)

---

## Worksheet Content

### Issue(s)
The data leak occurred because the manager failed to remove access permissions after sharing the folder. The employee later shared the wrong link containing internal files. Lack of proper access control and oversight led to public exposure of confidential documents.

### Review
NIST SP 800-53: AC-6 defines least privilege as limiting user access to only the information and resources necessary for their job duties. It emphasizes enforcing access restrictions and reviewing privileges regularly to minimize risks of unauthorized disclosure.

### Recommendation(s)
1. Implement automated access expiration for shared resources.  
2. Require managerial approval for external file-sharing links and apply classification-based access controls.

### Justification
Automated access expiration prevents old shared folders from remaining accessible after use. Approval-based sharing ensures oversight when external links are distributed. Both enhancements reduce the risk of unintentional exposure and align with NIST’s least privilege principles.

---

## What to Include in Your Response
- 2–3 sentences analyzing the factors that led to the incident  
- 2–3 sentences summarizing NIST SP 800-53: AC-6  
- 2 control enhancement recommendations to improve least privilege  
- 2–3 sentences justifying your recommendations

# Data leak worksheet

## https://docs.google.com/document/d/1ut3hjFmQC_204CqM3hNuy6mlVNcujNV6iuL9SusH8s8/edit?usp=sharing
