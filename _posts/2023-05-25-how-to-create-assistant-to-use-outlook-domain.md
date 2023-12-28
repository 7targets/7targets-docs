---
date: 2023-02-08
title: How to create assistant to use OUTLOOK domain.
# video_id: 6xyI5NNCCmc
description:  If you want your Assistant to send email from your company domain instead of `<yourcompany>.7ts-e.com `and your company domain email is on OUTLOOK for Business, then you can use this feature.
type: How-to
sidebar:
  - {id: overview-of-assistants, text: Overview of Assistants}
  - {id: usage-of-assistants, text: Usage of Assistants}
  - {id: step-1, text: Step 1}
  - {id: step-2, text: Step 2}
  - {id: step-3, text: Step 3}
  - {id: setting-spam-filter-for-deepali, text: Setting Spam Filter for Deepali}

categories:
  - How-To
# set: getting-started
# set_order: 3
---
If you want your Assistant to send email from your company domain instead of `<yourcompany>.7ts-e.com` and your company domain email is on OUTLOOK for Business, then you can use this feature.
As of now, you need 2 assistants in 7Targets to get this feature working.
Before you start, make sure that you have the email address for your assistant ready on your domain.
For e.g. If you want to use Deepali, make sure `Deepali@<yourcompany>`.com is already created. If such an email id does not exist, create it before moving to next steps. If you don’t have the rights to create email in your organization, please get in touch with your IT administrator to take his help to create the required email id.

## Overview of Assistants:
1st Assistant will have an email address that is on your domain. This assistant will be used for sending and receiving emails. Let me call her Deepali. `Deepali@<yourcompany>.com `
2nd Assistant will be used for composing messages, remembering the dates to send, processing the email responses, etc. Let me call this second assistant - John `John@<yourcompany>.7ts-e.com`. (Forwarder email address)

## Usage of Assistants :
You never have to worry about doing any specific settings for John (Forwarder email address). You have to work with Deepali Assistant only. John is used ONLY once in the entire process configuration, and that is for setting auto forwarding email address.
We will be setting an auto forwarding rule in Deepali’s OUTLOOK box to forward all incoming emails to John (Forwarder email address) .


## Step 1:
Login into 7Targets. Create an Assistant named John (Forwarder email address). Do NOT select the option I want to use my own domain. Go with the default settings and hit ‘Save’ assistant. Make sure you see John Assistant in your list of Assistants. 
## Step 2:
This step is where we will create the actual assistant which will use your domain.
In 7Targets, Click on Create a new Assistant . This time, make sure to select the option I want to use my own domain.

On clicking it, you would be asked to authorize the OUTLOOK account you want to use for the Assistant. From the popup, select Deepali’s account in your existing company email accounts.
![Outlook 1](../../images/outlook_image1.png)
![Outlook 2](../../images/outlook_image2.png)
![Outlook 3](../../images/outlook_image3.png)
![Outlook 4](../../images/outlook_image4.jpg)
![Outlook 5](../../images/outlook_image5.jpg)
![Outlook 6](../../images/outlook_image6.jpg)

Once Authorization is done,the following screen will be shown
We can verify the Assistant Deepali is created in Assistant’s Page.
![Outlook 8](../../images/outlook_image8.jpg)
## Step 3:
To start work on leads, you need to assign them to Deepali Assistant. To check status of leads, you can check it in Deepali Assistant. You can ignore John Assistant for all everyday usability purposes.  
  
## Setting Spam Filter for Deepali
If you see that valid responses to Deepali are landing into Deepali’s spam, we recommend you to set up the below email filter in Deepali’s OUTLOOK box.
1.	At the top of the page, select Settings > View all Outlook settings.
2.	Select Mail > Junk email.
3.	Under Safe senders, enter the email address or domain you want to add, and select Add.
4.	Select Save.
Assuming all Deepali’s email will have your company name, whenever Deepali receives a response, your company name will be in the response email as well. In all such cases, the email will not go into spam.
If an email goes into spam, the auto-forwarding rule is NOT triggered. Hence we need to ensure that auto-forwarding is triggered correctly. Without forwarding, 7Targets cannot process the received emails. Hence it’s important to set this step right.
![Outlook 9](../../images/outlook_image9.png)