# Activity Overview

In this activity, you will respond to a phishing incident involving a malicious file hash. This is the same SHA256 file hash that you investigated and verified as malicious in a previous activity. You'll follow playbook instructions to investigate and resolve the incident's alert ticket.

Previously, you learned how playbooks outline step-by-step actions necessary to respond to a security incident. Coordinated, effective, and quick action is critical during incident response. Playbooks guide security teams to minimize impact and reduce response time.

## Scenario

You are a level-one SOC analyst at a financial services company. You previously received a phishing alert about a suspicious file downloaded on an employee's computer. The attachment's hash has been verified as malicious. You must follow your organization's process to investigate and resolve the alert.

Your organization's security policies describe how to respond to specific alerts, including phishing alerts. Use the playbook flowchart and instructions to complete your investigation and update the alert ticket with your findings.

**Note:** Use the incident handler's journal from a previous activity to take notes.

---

## Step-By-Step Instructions

### Step 1: Access the template
Click the link and select Use Template:  
[Alert ticket](#)  

Or download the template directly from the provided attachment.

### Step 2: Access supporting materials
Open the supporting materials:  
[Phishing Playbook (with flowchart)](#)  

Or download the materials directly from the provided attachment.

Review the playbook instructions and flowchart. The instructions provide detailed steps for each stage in the flowchart. The flowchart gives a high-level visual overview of the sequence of actions.

In the Alert ticket template, set **Ticket status** to `Investigating`.

Since the phishing alert has already been received, begin with Step 2 in the playbook: **Evaluate the alert**. Create a new entry in your incident handler's journal to record the incident details.

---

### Evaluating the Alert Ticket
Examine these elements:

- **Alert severity:** Medium or High severity often requires escalation.
- **Sender details:** Check for inconsistencies that indicate phishing, such as mismatched sender name and email address.
- **Message body:** Look for grammatical errors or unusual language.
- **Attachments or links:** Identify malicious files or links that could steal information or execute malicious code.

After evaluation, answer the **5 W's**:

1. **Who** caused the incident?  
2. **What** happened?  
3. **When** did the incident take place?  
4. **Where** did the incident occur?  
5. **Why** did it happen?  

Record 2-3 reasons indicating whether the phishing alert is legitimate.

---

### Step 3: Analyze Email Details
Follow Steps 3.0 and 3.1 in the playbook:

- Determine if the email contains links or attachments.  
- Verify if these links or attachments are malicious.  
- In this case, the email contains a verified malicious attachment.  

If escalation is needed, proceed to Step 3.2; otherwise, move to Step 4.

---

### Step 4: Update Alert Ticket
Update the alert ticket based on your findings:

- **Ticket status:** Set to `Closed` or `Escalated`.  
- **Ticket comments:** Describe the steps taken and justify your decision. Include 2-3 reasons supporting why the ticket should be escalated or closed, using specific details from the alert.

---

## What to Include in Your Response

1. Update **Ticket status** in the Alert ticket dropdown.  
2. Provide a brief sentence describing the alert and what happened.  
3. Include 2-3 sentences explaining why you chose to escalate or close the ticket, supported with details from the alert ticket.

# Alert ticket
## https://docs.google.com/document/d/1ldxg4b10uxPO6JmhkYZ0UY_5RmTFWZgEIF5600D5l-Y/edit?usp=sharing


# Link to supporting materials
## https://docs.google.com/document/d/1rOSSCtLsiWVjAjTdJtWrSrvqpiXHissEAqiy5KD4Kv4/template/preview?usp=sharing
