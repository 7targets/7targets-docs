---
date: 2023-03-31
title: How to Enable Assistants to Use Your Own Subdomain for Sending Emails to Leads? 
# video_id: 6xyI5NNCCmc
description:  If you want your Assistant to send emails to the leads via your email subdomain then here are the step that you will need to follow.
type: How-to
#sidebar:

categories:
  - How-To
# set: getting-started
# set_order: 3
---

## Using Your Own Subdomain
7Targets utilizes AWS SES for sending out emails, and currently, we support the use of your own subdomain. To enable this feature, you need to grant us permission to use your subdomain by adding a DNS record to your DNS Server. Once this step is completed, we can proceed with creating an Assistant using your subdomain. The following steps outline the process:

1. We will need to create two Assistants for this process. One Assistant's email ID will belong to your subdomain, while the other Assistant will be a forwarder Assistant hosted on the 7Targets domain. For example, the forwarder Assistant could be 'shreya@7targets.7ts-e.com.'

2. Your Assistant must be created with a valid email ID from your subdomain. For instance, if your subdomain is 'stellar.com,' a valid email ID could be 'ashley@stellar.com' or 'roma@stellar.com.' The Assistant's name can be customized according to your preferences. You need to provide the email ID you have chosen for your Assistant to 7Targets.

3. Let's assume you have selected 'ashley@stellar.com' as the Assistant's email ID.

4. Once you provide this email ID to 7Targets, you will receive a verification link at the specified email address. Clicking on this link will verify your email ID and enable us to send emails to your leads.

5. Configure an auto-forwarding rule from your Assistant's email account (ashley@stellar.com). The recipient email address for auto-forwarding should be that of the forwarder Assistant (shreya@7targets.7ts-e.com).




