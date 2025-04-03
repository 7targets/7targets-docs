---
date: 2023-02-08
title: How to create assistant to use OUTLOOK domain
# video_id: 6xyI5NNCCmc
description: If you want your Assistant to send email from OUTLOOK for Business with your company domain, then you can use this feature.
type: How-to
sidebar:
  - {
      id: overview,
      text: Setting Up Your Email Assistant with Outlook Business,
    }
  - { id: create-assistant, text: Creating Your Outlook Assistant }
  - { id: verify-and-add-leads, text: Verify and Add Leads }
  - { id: forwarding-setup, text: Forwarding Setup for Outlook }
  - { id: setting-spam-filter, text: Setting Spam Filter }
  - { id: issues-that-happen, text: Issues that happen }

categories:
  - How-To
# set: getting-started
# set_order: 3
---

## Setting Up Your Email Assistant with Outlook Business

Want to easily send emails from your company's outlook business domain? This guide will show you how to set up a simple assistant that will handle sending and receiving emails.

We're creating an assistant that will use your company's email address (like `deepali@<yourcompany>.com`) to send emails from Outlook. This will make it super easy to followup with your leads.

## Creating Your Outlook Assistant

This guide will walk you through setting up an assistant that uses your own domain. Here's how to do it:

1.  **Navigate to Create a New Assistant:** In 7Targets, click on "Create a new Assistant."
2.  **Select Your Domain:** Make sure to choose the option that allows you to use _your own_ domain for this assistant.
3.  **Authorize the Account:** You'll be prompted to authorize the OUTLOOK account you want to use for this assistant. Select the right account (like a Deepali) from your existing company email.

![Outlook 1](../../images/outlook_image1.png)
![Outlook 2](../../images/outlook_image2.png)
![Outlook 3](../../images/outlook_image3.png)
![Outlook 4](../../images/outlook_image4.jpg)
![Outlook 5](../../images/outlook_image5.jpg)
![Outlook 6](../../images/outlook_image6.jpg)

Once Authorization is done, the following screen will be shown  
We can verify the Assistant Deepali is created in Assistant’s Page.
![Outlook 8](../../images/outlook_image8.jpg)

## Forwarding Setup for Outlook

If your Outlook email is routed through a third-party filtering service such as SpamExperts, Mimecast, or Avanan, you may need to set up a Forwarding Assistant to ensure emails are properly forwarded.

If your email does not use any third-party services, you can skip this step.

#### Step 1: Check Your MX Records

If you're unsure whether your Outlook email is using a third-party filtering service, follow these steps:

1. Log in to your domain's DNS provider (e.g., GoDaddy, Cloudflare, Namecheap, etc.).

2. Locate the MX (Mail Exchange) Records section.

3. Look for entries like:

- mail.protection.outlook.com → **No third-party filtering** (Microsoft 365 default).

- _.mimecast.com, _.spamexperts.net, \*.avanan.com → **Third-party filtering is active**.

4. If you see third-party filtering, proceed with setting up the Forwarding Assistant.

#### Step 2: Create a Forwarding Assistant in 7Targets

1. Log in to your 7Targets account.

2. Navigate to Assistants and click on Create a New Forwarder Assistant.

3. Copy the forwarder email address generated for your assistant.

#### Step 3: Set Up Email Forwarding in Outlook

1. Sign in to your Outlook account.

2. Go to Settings (⚙️) > View all Outlook settings.

3. Navigate to Mail > Forwarding.

4. Enable Forward my email to and enter the Forwarder Assistant’s email address from 7Targets.

5. (Optional) Check Keep a copy of forwarded messages if needed.

You're All Set!
Your Outlook account will now automatically forward emails to the 7Targets Assistant.

## Setting Spam Filter

We recommend you to set up the below email filter in Deepali’s OUTLOOK box so avoid responses to land in Spam.

1. At the top of the page, select Settings > View all Outlook settings.
2. Select Mail > Junk email.
3. Under Safe senders, enter the email address or domain you want to add, and select Add.
4. Select Save.

## Verify and Add Leads

Edit the Assistant and click on "Send Test Email" to verify if the Assistant is working fine.  
To start work on leads, you need to add leads for the newly created Assistant. To check status of leads, you can check it in Assistant.

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
