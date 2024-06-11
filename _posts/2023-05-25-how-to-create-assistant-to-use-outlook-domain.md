---
date: 2023-02-08
title: How to create assistant to use OUTLOOK domain
# video_id: 6xyI5NNCCmc
description:  If you want your Assistant to send email from OUTLOOK for Business with your company domain, then you can use this feature.
type: How-to
sidebar:
  - {id: overview, text: Overview}
  - {id: create-assistant, text: Create Assistant}
  - {id: verify-and-add-leads, text: Verify and Add Leads}
  - {id: setting-spam-filter, text: Setting Spam Filter}
  - {id: issues-that-happen , text: Issues that happen}

categories:
  - How-To
# set: getting-started
# set_order: 3
---
If you want your Assistant to send email from your company domain on OUTLOOK for Business, then you can use this feature.  

## Overview:
Assistant will have an email address that is on your domain. This assistant will be used for sending and receiving emails. Lets say `Deepali@<yourcompany>.com `

## Create Assistant:
This step is where we will create the assistant which will use your domain.  
In 7Targets, Click on Create a new Assistant. Make sure to select the option I want to use my own domain.

On clicking it, you would be asked to authorize the OUTLOOK account you want to use for the Assistant. From the popup, select right (e.g. Deepali’s) account in your existing company email accounts.
![Outlook 1](../../images/outlook_image1.png)
![Outlook 2](../../images/outlook_image2.png)
![Outlook 3](../../images/outlook_image3.png)
![Outlook 4](../../images/outlook_image4.jpg)
![Outlook 5](../../images/outlook_image5.jpg)
![Outlook 6](../../images/outlook_image6.jpg)

Once Authorization is done, the following screen will be shown  
We can verify the Assistant Deepali is created in Assistant’s Page. 
![Outlook 8](../../images/outlook_image8.jpg)

## Verify and Add Leads
Edit the Assistant and click on "Send Test Email" to verify if the Assistant is working fine.  
To start work on leads, you need to add leads for the newly created Assistant. To check status of leads, you can check it in Assistant. 

## Setting Spam Filter
We recommend you to set up the below email filter in Deepali’s OUTLOOK box so avoid responses to land in Spam.
1.	At the top of the page, select Settings > View all Outlook settings.
2.	Select Mail > Junk email.
3.	Under Safe senders, enter the email address or domain you want to add, and select Add.
4.	Select Save.

Assuming all Deepali’s email will have your company name, whenever Deepali receives a response, your company name will be in the response email as well. In all such cases, the email will not go into spam. 

If an email goes into spam, that email will not be read by the Assistant. 

![Outlook 9](../../images/outlook_image9.png)

## Issues that happen 
**Important**
You are giving access of one of the email boxes (Deepali in this case), to 7Targets. 
You are authorizing 7Targets to access this email box for reading and writing emails. 
You will have to REAUTHORIZE this every 90 days. 
It's not a good practice to allow another company to use a email box forever. Hence Microsoft enforces this REAUTHORIZATION every 90 days. 
The Assistant Deepali will remind you via email whenever she is unable to send emails because she was not allowed to send emails after 90 days. 

![image](../../images/microsoft-block-account.png)

Here is the microsoft link on this: https://learn.microsoft.com/en-us/azure/active-directory/develop/refresh-tokens#refresh-token-expiration 