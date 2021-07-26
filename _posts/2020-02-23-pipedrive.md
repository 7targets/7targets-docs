---
date: 2020-02-23
title: Pipedrive  
description: Integrate 7Targets AI Assistant with Pipedrive 
type: Document
sidebar:
  - {id: what-you-get, text: What you get}
  - {id: authorize-pipedrive-for-7targets, text: Authorize Pipedrive for 7Targets}
categories:
  - integrate
---

<a name="what-you-get"/>
## [What you get](#what-you-get)
Deals from **Pipedrive** CRM can be assigned to 7Targets AI Sales Assistant directly within the Pipedrive UI. AI Assistant will then own the lead and communicate to try and get the meeting. Assistant will also update the deal by putting notes for the emails being sent.

One **important** point to note, as soon as the AI Assistant receives a response from the lead and detects it to be a Hot or Responded lead then the assistant assigns the lead back to the original owner.

For onboarding your AI Assistant on Pipedrive please reach out to support@7targets.com

## Authorize Pipedrive for 7Targets
**Authorize Pipedrive** by clicking this link [authorize](https://solution.7targets.com/pipedrive-authorize){:target="_blank" rel="noopener"}. Once Authorization is complete follow below steps for further configuration before it is ready to be used. 

1. Create your assistant in 7Targets if not already created. Provide the default values for context and other variables at the Assistant level by editing the Assistant.  

2. Create a user in Pipedrive for your Assistant's email id.  

3. In 7Targets, under user profile, look at the "CRM Details" tab and click on "Verify Again" to get the acceptable status. Various status and the meanings are below:   
**ASSISTANT_EXISTS_AS_USER_IN_CRM** : You are all set. Go ahead and assign one contact from Pipedrive to the Assistant user in Pipedrive. That contact should be seen as lead in 7Targets in few seconds.  
**ASSISTANT_DOES_NOT_EXISTS_AS_USER_IN_CRM** : Follow step 2 and beyond above.  
**ASSISTANT_NOT_YET_CREATED** : Follow Step 1 onwards.  
**ALL_WORKING_WELL** : All set, it is working well for you.  

4. In Pipedrive, disable email notifications for the Assistant user.  

5. Verify in 7Targets that your Assistant has a Default Context. It is available on Edit Assistant page.

6. You are set, assign a contact/lead in Pipedrive to the Assistant user and verify that you see that lead in 7Targets in the "Leads" page. 

7.  If you intend to pass context to the lead from Pipedrive then create a custom field named "context" for Contacts in Pipedrive. With this, when you assign the contact/lead to Assistant user and if there is any context provided for this contact/lead then Assistant will use that else it will use the default context provided at the Assistant level in 7Targets. 
