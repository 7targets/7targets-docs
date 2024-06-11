---
date: 2023-02-08
title: How to create assistant to use GMAIL domain
# video_id: 6xyI5NNCCmc
description:  If you want your Assistant to send email from your company domain email on GMAIL for Business, then you can use this feature.
type: How-to
sidebar:
  - {id: tldr, text: TL;DR}
  - {id: overview-of-assistants, text: Overview of Assistants}
  - {id: usage-of-assistants, text: Usage of Assistants}
  - {id: 1-create-forwarder-assistant, text: 1. Create Forwarder Assistant}
  - {id: 2-create-mia-assistant, text: 2. Create Mia Assistant}
  - {id: 3-authorization-and-configuration, text: 3. Authorization and Configuration}
  - {id: 4-auto-forwarding-setup, text: 4. Auto Forwarding Setup}
  - {id: 5-setting-spam-filter-for-mia, text: 5. Setting Spam Filter for Mia}

categories:
  - How-To
# set: getting-started
# set_order: 3
---

## TL;DR
Simplified Email Integration with Your Company Domain on 7Targets for GMAIL

### Objective
* Enable Assistant to use your company domain for emails.
* Use two Assistants: Mia@<yourcompany>.com for emails, and Forwarder@<yourcompany>.7ts-e.com for backend processes.

### Step 1: Create Forwarder Assistant
* In 7Targets, create Forwarder Assistant without your domain.

### Step 2: Create Mia Assistant
* Create Mia with "I want to use my own domain" option.
* Authorize Mia's GMAIL account.

### Step 3: Authorization and Configuration
* Verify Mia's creation in 7Targets.
* Configure auto-forwarding in Mia's GMAIL to Forwarder.

### Step 4: Auto Forwarding Setup and Spam Filter
* Set auto forward in Mia's GMAIL to Forwarder's email.
* Confirm auto forward for activation.
* Configure GMAIL filter for Mia to prevent valid responses from going to spam.

-------------------------------------

## Details 
If you want your Assistant to send email from your company domain instead of `<yourcompany>.7ts-e.com `and your company domain email is on GMAIL for Business, then you can use this feature.  
As of now, you need 2 assistants in 7Targets to get this feature working.  

Before you start, make sure that you have the email address for your assistant ready on your domain.  
For e.g. If you want to use Mia, make sure `Mia@<yourcompany>.com `is already created.  
If such an email id does not exist, create it before moving to next steps. 

If you don’t have the rights to create email in your organization, please get in touch with your IT administrator to take his help to create the required email id. 

## Overview of Assistants:
1st Assistant will have an email address that is on your domain. This assistant will be used for sending and receiving emails. Let me call her Mia. `Mia@<yourcompany>.com`  

2nd Assistant will be used for composing messages, remembering the dates to send, processing the email responses, etc. Let me call this second assistant - Forwarder `Forwarder@<yourcompany>.7ts-e.com`. 

## Usage of Assistants:
You never have to worry about doing any specific settings for Forwarder. You have to work with Mia Assistant only. Forwarder is used ONLY once in the entire process configuration, and that is for setting auto forwarding email address.  
We will be setting an auto forwarding rule in Mia’s GMAIL box to forward all incoming emails to Forwarder.

## 1: Create Forwarder Assistant
Login into 7Targets.  
Create an Assistant named Forwarder. **Do NOT select the option I want to use my own domain**.  
Go with the default settings and hit ‘Save’ assistant. 

Make sure you see Forwarder Assistant in your list of Assistants.
## 2: Create Mia Assistant
This step is where we will create the actual assistant which will use your domain.  
In 7Targets, Click on Create a new Assistant.  
This time, make sure to select the option `I want to use my own domain`.  
On clicking it, you would be asked to authorize the gmail account you want to use for the Assistant.  
From the popup, select Mia’s account in your existing company email accounts.  
![Outlook 1](../../images/outlook_image1.png)
![Outlook 2](../../images/outlook_image2.png)

## 3: Authorization and Configuration
Once Authorization is done,the following screen will be shown  
![Gmail 1](../../images/gmail_image3.png)  
We can verify the Assistant Mia is created in Assistant’s Page.  
![Gmail 2](../../images/gmail_image4.png)  
After authorizing, you have to configure below mentioned steps  
## 4: Auto Forwarding Setup
1.	Log into to Mia’s Gmail account.
![Gmail 5](../../images/gmail_image5.png)
![Gmail 6](../../images/gmail_image6.png)
2.	Configure auto forwarding (Under Gmail Settings->All Settings->Forwarding and POP/IMAP).
![Gmail 7](../../images/gmail_image7.png)
3.	Set the auto forward to send the received emails to Forwarder email address `Forwarder@<yourcompany>.7ts-e.com`. To ensure there are no spelling mistakes, you can copy Forwarder's email from the 7Targets->Assistants page using `Copy Email Address` link.
![Gmail 8](../../images/gmail_image8.png)
![Gmail 9](../../images/gmail_image9.png)
4.	You will receive an email to confirm the autoforward. Make sure to confirm by clicking on the link or using the code as mentioned in that email, else it will not work.
![Gmail 10](../../images/gmail_image10.png)

![Gmail 11](../../images/gmail_image11.png)

![Gmail 12](../../images/gmail_image12.png)

![Gmail 13](../../images/gmail_image13.png)

To start work on leads, you need to assign them to Mia Assistant. To check status of leads, you can check it in Mia Assistant. You can ignore Forwarder Assistant for all everyday usability purposes.  
## 5: Setting Spam Filter for Mia
If you see that valid responses to Mia are landing into Mia’s spam, we recommend you to set up the below email filter in Mia’s GMail box.
1.	Go to GMail Settings
2.	Go to “Filters and Blocked Addresses”
3.	Click “Create a New Filter”
4.	Choose “Has the words”.
5.	Add in that list of words. If your company name is Callify.ai, add “Callify” in “Has the words” section.
6.	In the actions for this filter, select “Never send it to spam”
7.	Save the filter.  

Assuming all Mia’s email will have your company name, whenever Mia receives a response, your company name will be in the response email as well. In all such cases, the email will not go into spam.  

If an email goes into spam, the auto-forwarding rule is NOT triggered. Hence we need to ensure that auto-forwarding is triggered correctly. Without auto-forwarding, 7Targets cannot process the received emails. Hence it’s important to set this step right.


