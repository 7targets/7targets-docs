---
date: 2023-02-14
title: How to add an Assistant that connects with Exchange Server Outlook email id
# video_id: 6xyI5NNCCmc
description: This post describes the steps on how you can add a new email id and connect it with a 7Targets AI Assistant. This enables all email communications to go via your email account. 
type: How-to
sidebar:
  - {id: Click-on-Add-Assistant, text: Click on Add Assistant }
  - {id: Use-my-own-domain, text: Use my own domain } 
  - {id: Authorize-7Targets-to-use-Exchange-email-box, text: Authorize 7Targets to use Exchange email box } 
  - {id: Send-test-email, text: Send test email } 
  
categories:
  - How-To
# set: getting-started
# set_order: 3
---

## Create a new email id in your Exchange Server
Decide the name of your assistant and create that email id in your corporate exchange server. 
For example: lets assume the assistant name is Emma. And your company is abccorp.com
Create Emma@abccorp.com

## Click on Add Assistant
Open 7Targets. 
Go to the Assistants top menu. 
And click on 'Add Assistant' button. 
Dont worry about giving a name to this assistant, because Assistant will pick up Emma's name directly from your exchange server email id.  

## Use my own domain
Scroll down, Click on 'Use my own domain' - a green colored check box. 
Choose Exchange Server from the following popup. 
MAKE SURE you select Emma assistant email address account in Exchange server. 

Do NOT select your own email account. 

## Authorize 7Targets to use Exchange email box
Once you select Emma@abccorp.com, it will ask you to approve and authorize 7Targets to allow connection with Emma's email box. 7Targets needs READ and WRITE access to Emma's box so it can work as an assistant, like any other human assistant. 

Provide those permissions. 

## Send test email
Go to Custom Messages, select a custom message, and send test email. 
Make sure you see the Emma Assistant in the top icon's. This ensures that Emma assistant is selected while sending the email. 

## Issues that happen 
**Important**
You are giving access of one of the email boxes (Emma in this case), to 7Targets. 
You are authorizing 7Targets to access this email box for reading and writing emails. 
You will have to REAUTHORIZE this every 90 days. 
It's not a good practice to allow another company to use a email box forever. Hence Microsoft enforces this REAUTHORIZATION every 90 days. 
The Assistant Emma will remind you via email whenever she is unable to send emails because she was not allowed to send emails after 90 days. 

![image](../../images/microsoft-block-account.png)

Here is the microsoft link on this: https://learn.microsoft.com/en-us/azure/active-directory/develop/refresh-tokens#refresh-token-expiration 

If you have any further doubts, you can directly mail us at support@7targets.com.

