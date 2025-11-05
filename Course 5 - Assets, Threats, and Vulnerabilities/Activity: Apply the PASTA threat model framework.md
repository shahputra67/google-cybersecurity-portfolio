# Activity Overview

In this activity, you will practice using the Process of Attack Simulation and Threat Analysis (PASTA) threat model framework. You will determine whether a new shopping app is safe to launch.

Threat modeling is an important part of secure software development. Security teams typically perform threat models to identify vulnerabilities before malicious actors do. PASTA is a commonly used framework for assessing the risk profile of new applications.

## Scenario

You’re part of the growing security team at a company for sneaker enthusiasts and collectors. The business is preparing to launch a mobile app that makes it easy for their customers to buy and sell shoes.

You are performing a threat model of the application using the PASTA framework. You will go through each of the seven stages of the framework to identify security requirements for the new sneaker company app.

## Step-By-Step Instructions

Follow the instructions and answer the included questions to complete the activity.

### Part 1 - Access the Resources

To use the template for this course item, click the following link and select **Use Template**:  

[PASTA worksheet](#)

OR  

If you don’t have a Google account, you can download the template directly from the attachment.

Supporting materials:  

PASTA data flow diagram: [https://docs.google.com/presentation/d/1ol7y79popTFfNHM-90ES-H-i1Lpd0YNvPShxBlXozjg/template/preview?resourcekey=0-DZAkf7Vzh2PXsP-j3oXV-g](#)

PASTA attack tree: [https://docs.google.com/presentation/d/1FmWLyHgmq9XQoVuMxOym2PHO8IuedCkan4moYnI-EJ0/template/preview?resourcekey=0-zYPY7AhPJdcClXamlAfOag#slide=id.p](#)


### Part 2 - Complete the PASTA Stages

#### Stage I – Business Objectives

The main goal of Stage I of the PASTA framework is to understand why the application was developed and what it is expected to do. Stage I typically requires input from many individuals at the business.

**Description:**  
Our application should seamlessly connect sellers and shoppers. It should be easy for users to sign-up, log in, and manage their accounts. Data privacy is a big concern. Buyers should be able to message sellers and rate them. Sales should be clear and quick, with several payment options. Proper payment handling is important to avoid legal issues.

**Task:**  
In the Stage I row of the PASTA worksheet, make 2-3 notes of business objectives from the description.

#### Stage II – Technological Scope

Stage II defines the technological scope of the project. The development team is involved because they understand the code base and logic. Your role is to evaluate the application's architecture for security risks.

**Technologies:**

- **API**: Defines how software components interact. Third-party APIs add functionality without custom code.  
- **PKI (AES & RSA)**: Encrypts sensitive data and exchanges keys securely.  
- **SHA-256**: Hash function to protect passwords and sensitive user data.  
- **SQL**: Stores and retrieves sneaker and seller information during purchases.

**Task:**  
Decide which technology to evaluate first and why. In Stage II of the worksheet, write 2-3 sentences (40-60 words) explaining your choice.

#### Stage III – Application Analysis

Stage III analyzes how the application handles information. Each process is broken down. For example, buyers searching the database for sneakers.

**Task:**  
Open the PASTA data flow diagram and consider how the technologies you prioritized protect user data during these processes.

#### Stage IV – Threat Identification

Stage IV identifies potential threats to the application, including those affecting technologies from Stage II and processes from Stage III. For example, the authentication system could be attacked via malware or social engineering.

**Task:**  
In Stage IV of the worksheet, list 2 types of threats that could impact the sneaker app.

#### Stage V – Vulnerability Analysis

Stage V considers the attack surface of technologies. For example, a payment form could be vulnerable if it fails to encrypt credit card information.

**Task:**  
In Stage V of the worksheet, list 2 vulnerabilities that could be exploited. Resources like the CVE® list and OWASP help identify common vulnerabilities.

#### Stage VI – Attack Modeling

Stage VI uses the information from previous steps to build an attack tree. Review the PASTA attack tree and consider how threat actors might exploit vulnerabilities.

#### Stage VII – Security Controls

Stage VII focuses on implementing defenses to mitigate threats.  

**Task:**  
In Stage VII of the worksheet, list 4 security controls that reduce the chances of incidents like data breaches.

## What to Include in Your Response

- 2-3 business objectives  
- 2-3 technology requirements  
- 2 potential threats  
- 2 system vulnerabilities  
- 4 defenses to limit risk

## PASTA worksheet

### https://docs.google.com/document/d/1sZmp_2cWVvl1_eY1w0E3uhE0XwF6MW9Z5cMnf9qKiiM/edit?usp=sharing
