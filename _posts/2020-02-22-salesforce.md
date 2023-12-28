---
date: 2020-02-22
title: Salesforce 
description: Assign Leads or Contacts from Salesforce to 7Targets AI Assistant. Assistant will followup and log the email too in Salesforce. 
type: Document
sidebar:
  - {id: what-you-get, text: What you get}
  - {id: configure-salesforce, text: Configure Salesforce}
  - {id: configure-7targets, text: Add Salesforce Credentials in 7Targets }
categories:
  - integrate
---

## What you get
Leads from **Salesforce** CRM can be assigned to 7Targets AI Sales Assistant directly within the Salesforce UI. AI Assistant will then own the lead and nurture to try and get the meeting. Assistant will also update Salesforce putting notes for the emails being sent as well as status of the lead in salesforce. 

## Configure Salesforce
1. Goto _Setup_ > _Object Manager_ > search _Lead_ in Quick Find Box.
1. In _Lead_ Object go to _Fields & Relationships_ > Click on _New_ button to create following three new fields 
![Assistant Email](../../images/salesforce_assistant_email.png)

![Seven Targets State](../../images/salesforce_seven_targets_state.png)

![Seven Targets Sequence](../../images/salesforce_seven_targets_sequence.png)

1. In _Lead_ Object go to _Triggers_ > Click on _New_ button to create new Trigger called LeadTrigger. You can find the code [here](https://github.com/7targets/Salesforce-Integration/blob/main/LeadTrigger.tgr)
1. In _Setup_ search for _Apex Classes_ & create a new Apex Class called SevenTargetsLeadIntegration. You can find the code [here](https://github.com/7targets/Salesforce-Integration/blob/main/SevenTargetsLeadIntegration.cls)
1. Make sure you check the following checkbox for each Field
![Restrict Picklist](../../images/restrict_picklist.png)
1. Goto _Setup_ > search _custom setting_ in Quick Find Box.
1. In _Custom Setting_ create a new setting as shown below.
![Seven Targets API](../../images/salesforce_seven_targets_api.png)
1. In Newly Created Above custom setting add below fields.
![Seven Targets API Fields](../../images/salesforce_seven_targets_api_fields.png)
1. You can get Client Id & Client Secret from support@7targets.com
1. If you don't have existing Certificate & Private Key then generate one from [here](https://developer.salesforce.com/docs/atlas.en-us.246.0.sfdx_dev.meta/sfdx_dev/sfdx_dev_auth_key_and_cert.htm?_ga=2.43114208.439795187.1656333652-1742453021.1655933163).
1. Create a Connected App in Salesforce using steps given [here](https://help.salesforce.com/s/articleView?id=sf.task_create_connected_app.htm&type=5). Copy Consumer key given which will be used in further setup.

## Add Salesforce Credentials in 7Targets
1. In 7targets go to the _CRM_ page using menu bar from left side.
2. Add username(in the form of email), consumer key and private key. This will be used while connecting with Salesforce API.

For any help fell free to drop us an email at support@7targets.com