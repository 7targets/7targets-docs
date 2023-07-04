---
date: 2020-01-02
title: Create your Assistant
video_id: cHU_bPKqZSg
description: Create your Virtual Assistant 
type: Video
sidebar:
  - {id: add-assistant, text: Add Assistant}
  - {id: use-own-domain, text: Use Own Domain}
  - {id: use-exchange-server, text: Use Exchange Server}
  - {id: use-gmail, text: Use Gmail}
  - {id: questions-answered, text: Questions answered}
categories:
  - getting-started
set: getting-started
set_order: 2
---

## Add Assistant

Your Assistant is identified by name, email address and title. It is `recommended to have a geography specific name` for better connect with your leads, for e.g. Ashley or John will be able to connect better in the Americas. You can always change the name later.

Let’s pick or type an appropriate title. 

Company name is used by the Assistant in the AI generated email subjects. Assistant’s email address too is derived from the company name. You can change the Company name and email address of Assistant later.

Note the generated signature. You can always edit the signature later.

Some of our customers use the Assistant title as “Executive Assistant to self”. While some use Assistant’s name as their own name. It is your choice finally. 

Click the button to create your Assistant and go to the next step.

## Use Own Domain
Can I use my email or my domain as Assistant Email ?  
Yes, you can and it comes with risking your domain as well limits of your email server.  
We cannot do a apparent `from` for your email/domain and do a `reply-to` to assistants email id. As it would mean different domain for `from` and `reply-to`, which impacts the email deliverability. 

If you want to use your own domain+email as Assistants email address then we support it for Exchange Server and GMAIL for Business. Steps are mentioned below. 

**If you still want to use this feature, we highly recommend to create a new email-id on your email server and use that for the Assistant.**  

## Use Exchange Server
Here are the steps to use Exchange Server. 

https://7targets.ai/help/how-to/how-to-add-assistant-in-Exchange-Server-Outlook/


## Use Gmail
If you want your Assistant to send email from your company domain instead of `<yourcompany>.7ts-e.com` and your company domain email is on GMAIL for Business, then you can use this feature.  

As of now, you need 2 assistants in 7Targets to get this feature working.  
Before you start, make sure that you have the email address for your assistant ready on your domain.  
For e.g. If you want to use Ashley, make sure `Ashley@<yourcompany>.com` is already created. If such an email id does not exist, create it before moving to next steps. If you don't have the rights to create email in your organization, please get in touch with your IT administrator to take his help to create the required email id.  

**Overview :**  
**1st Assistant** will have an email address that is on your domain. This assistant will be used for sending and receiving emails. Let me call her `Ashley. Ashley@<yourcompany>.com`   
**2nd Assistant** will be used for composing messages, remembering the dates to send, processing the email responses, etc. Let me call this second assistant - `John John@<yourcompany>.7ts-e.com`.  

**Usage :**  
You never have to worry about doing any specific settings for John. You have to work with Ashley Assistant only. John is used *ONLY* once in the entire process configuration, and that is for setting auto forwarding email address.  
We will be setting an auto forwarding rule in Ashley’s GMAIL box to forward all incoming emails to John.  
*Let’s get started*  
*Step 1*: Login into 7Targets. Create an Assistant named John. Do **NOT** select the option I want to use my own domain. Go with the default settings and hit ‘Save’ assistant. Make sure you see John Assistant in your list of Assistants.  
*Step 2*: This step is where we will create the actual assistant which will use your domain.  
2.1. In 7Targets, Click on Create a new Assistant . This time, make sure to select the option I want to use my own domain.  
2.2. On clicking it, you would be asked to authorize the gmail account you want to use for the Assistant. From the popup, select Ashley’s account in your existing company email accounts.  
*After authorizing, you have to configure below mentioned step:*  
1. Log into to Ashleys Gmail account. 
1. Configure auto forwarding (Under Gmail Settings->All Settings->Forwarding and POP/IMAP). 
1. Set the auto forward to send the received emails to John email address John@<yourcompany>.7ts-e.com. To ensure there are no spelling mistakes, you can copy Johns email from the 7Targets->Assistants page using `Copy Email Address` link. 
1. You will receive an email to confirm the autoforward. Make sure to confirm by clicking on the link or using the code as mentioned in that email, else it will not work. 

To start work on leads, you need to assign them to Ashley Assistant. To check status of leads, you can check it in Ashley Assistant. You can ignore John Assistant for all everyday usability purposes. 

*Setting Spam Filter for Ashley*  
If you see that valid responses to Ashley are landing into Ashleys spam, we recommend you to set up the below email filter in Ashley’s GMail box. 
1. Go to GMail Settings
1. Go to “Filters and Blocked Addresses”
1. Click “Create a New Filter”
1. Choose “Has the words”.
1. Add <your company name> in that list of words. If your company name is Callify.ai, add “Callify” in “Has the words” section.
1. In the actions for this filter, select “Never send it to spam” 
1. Save the filter. 

Assuming all Ashley’s email will have your company name, whenever Ashley receives a response, your company name will be in the response email as well. In all such cases, the email will not go into spam.  
If an email goes into spam, the auto-forwarding rule is NOT triggered. Hence we need to ensure that auto-forwarding is triggered correctly. Without auto-forwarding, 7Targets cannot process the received emails. Hence it's important to set this step right. 

*Let's test it now*
1. Go to add a lead screen in 7Targets, and try adding one lead abc@xyz.com(this is just example, provide a valid email) to Ashley. 
1. Make sure you select ‘Now’, to ensure you can test the email has gone out immediately. 
1. Check if the abc got the email. 
1. Have abc reply to the email “I am interested. Call me”. 
1. Give it a couple of minutes and check if Ashleys lead list shows abc as a HOT lead. 
1. If you don’t see abc's response in 7Targets, check if abc@xyz.com response email has landed into the spam folder in Ashley’s GMail box. 
1. If it’s in the spam folder, then your spam rule in the above steps need to be set properly once again. 

## Questions answered
- What should be the Assistant name ? 
- Can I change Assistant name later ?
- What should be the Assistant title ? 
- Can I change the Assistant signature later ? 
- Can I use my email or my domain as Assistant Email ?

