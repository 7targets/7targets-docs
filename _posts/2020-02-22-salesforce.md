---
date: 2020-02-22
title: Salesforce 
description: Assign Leads or Contacts from Salesforce to 7Targets AI Assistant. Assistant will followup and log the email too. 
type: Document
sidebar:
  - {id: what-you-get, text: What you get}
  - {id: configure-assistant, text: Configure Assistant}
  - {id: create-zap, text: Create Zap}
categories:
  - integrate
---

## What you get
Leads from **Salesforce** CRM can be assigned to 7Targets AI Sales Assistant directly within the Salesforce UI. AI Assistant will then own the lead and communicate to try and get the meeting. Assistant will also update the lead details putting notes for the emails being sent as well as status of the lead in salesforce. 

## Configure Assistant
Provided the preferences for the assistant so that the Assistant can bcc the email being sent and it gets logged in CRM. Also assistant can forward any response received from the lead for it to be logged in the CRM.

![CRM Email Addresses](../../images/crm-bcc-and-forward-emailid.png)

## Create Zap
Now create a Zap to Assign the Lead or Contact from Salesforce to 7Targets.   
The Zapier 7Targets Integration is still private and is not yet on the Zapier public marketplace. So you can access it via this [private link](https://zapier.com/developer/public-invite/73649/157f0098ab326f339526b19ff7de5526/)   


## Directly use 7Targets API
If you want to avoid going via Zapier, you can call the 7Targets API to create or update the lead directly from Salesforce. Refere Salesforce documents on how to call some external API from within Salesforce.   
Details on 7Targets API are [here](../api)

One **important** point to note, as soon as the AI Assistant receives a response from the lead and detects it to be a Hot or Responded the assistant assigns the lead back to the original owner.

For onboarding your AI Assistant on Salesforce please reach out to support@7targets.com