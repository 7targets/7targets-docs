---
date: 2024-08-01
title: Reauthorize existing Assistant
video_id: ????????
description: How to reauthorize existing gmail or outlook assistant.
type: Video
sidebar:
  - {id: why-reauthorize, text: Why do I need to Reauthorize My Assistant}
  - {id: how-to-reauthorize, text: How do I Reauthorize My Assistant}
categories:
  - How-To
---

<a name="why-reauthorize"/>
## Why do I need to Reauthorize

When Assistant is created using Gmail or Outlook Service, it provides a refresh token which helps in connecting with respective services while sending or receiving emails.

After certain time period this refresh token expires and to continue the usage of these services user need to relogin and restore access with new refresh token.

You can find more details regarding these tokens below:
- [Microsoft](https://learn.microsoft.com/en-us/entra/identity-platform/refresh-tokens)
- [Gmail](https://developers.google.com/identity/protocols/oauth2)

<a name="how-to-reauthorize"/>
## How do I Reauthorize My Assistant
To Identify and Reauthorize you assistant you simply need to go to the Assistants Page and look for **Re-authorize** button.

![Reauthorize](../../images/reauthorize.png)

If an assistant is showing re-authorize button as shown in above image, you can click that button and it will ask for login details for that assistant's (Gmail/Outlook) account. After you login it might ask you for a confirmation.

After Successful Re-Authorization you will see notification similar to below image in top right corner.

![Reauthorization Successful](../../images/reuathorization_successful.png)

There might be some leads which failed to send Followups during the time when assistant was Un-authorized. To take care of these leads you will see a Pop-up similar to following. You have select desired Date & Time and Click on Yes and assistant will continue followup for those failed Lead's Followups.

![Continue Followup](../../images/continue_followup.png)