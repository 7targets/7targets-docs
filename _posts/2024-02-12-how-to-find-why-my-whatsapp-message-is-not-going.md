---
date: 2024-02-12
title: How to find out why Whatsapp message from Sequence is not going
description: Whatsapp message from the sequence may fail to actually go and there may be different reasons
# video_id: TcibhmCn9gM
type: How-to

sidebar:
  - {id: message-provider-configuration, text: Message provider configuration}
  - {id: whatsapp-message, text: WhatsApp Message}
categories:
  - How-To
# set: getting-started
# set_order: 3
---

## Message provider configuration
First thing to check is the Message provider configuration. 
1. You may not have created a default message provider
1. The sender phone number is not approved sender

There is a status and status details which provides the reasons. 
**Solution** is to correct the configuration and save the message provider.
After saving you can confirm if the leads which are impacted because of this provider configuration can/should be continued followup.

## WhatsApp Message
Listing the whatsapp message issues below. 
1. You may not be using an approved template with correct template id. 
1. The variable in the template may not be mapped to the right variable from 7Targets.
1. The sorrounding brackets `{{ }}` may not be correct. Like extra or less brackets around the variable.
1. There may no or extra mapping sign `->` that got added or removed while saving

Feel free to reach out to support@7targets.com for any assistance required during setup.
