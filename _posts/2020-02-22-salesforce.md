---
date: 2020-02-22
title: Integrate Salesforce with 7Targets AI Assistants
description: Assign Leads from Salesforce to 7Targets AI Assistant. Assistant will followup and log the emails in Salesforce. 
type: Document
sidebar:
  - {id: tl-dr, text: TL;DR} 
  - {id: what-you-get, text: What you get}
  - {id: configure-salesforce, text: Configure Salesforce}
  - {id: configure-7targets, text: Configure 7Targets }
categories:
  - integrate
---

## TL;DR 
Simplified Configuration steps for 7Targets AI Sales Assistant Integration with Salesforce
### 1. Salesforce Setup:
  * Add custom fields to the Lead Object: Assistant Email, Lead State, Sequence Name.
  * Create a new Trigger named LeadTriggerFor7Targets.
  * Create an Apex class SevenTargetsLeadIntegration.
  * Configure 7Targets API credentials in Salesforce Custom Metadata.

### 2. Connected App in Salesforce:
  * Generate a Certificate & Private Key if not available.
  * Create a Connected App in Salesforce and note the Consumer Key.

### 3. 7Targets Configuration:
  * Access the CRM page in 7Targets.
  * Add Salesforce username, Consumer Key, and Base64-encoded (can use use base64encode.org) Private Key.
  * Verify credentials using the Test button.

--------------------------------------------------------

# Details Steps with screen shots
## What you get
Leads from **Salesforce** CRM can be assigned to 7Targets AI Sales Assistant directly within the Salesforce UI. 
AI Assistant will then own the lead and nurture to try and get the meeting. Assistant will also update Salesforce putting notes for the emails being sent as well as status of the lead in salesforce. 

## Configure Salesforce
### Add custom fields in the Lead Object in Salesforce
Below three custom fields are to be added to the Lead Object.   

| Field Label  | Field Name | Data Type |
| -------- | ------- | ------- |
| 7Targets Assistant Email  | sts_assistant_email | Picklist |
| 7Targets Lead State | sts_lead_state | Picklist |
| 7Targets Sequence Name  | sts_sequence_name | Picklist |

1. Goto _Setup_ > _Object Manager_ > search _Lead_ in Quick Find Box.
1. In _Lead_ Object go to _Fields & Relationships_ > Click on _New_ button to create three new fields as in screen shots below.
![Assistant Email](../../images/salesforce_assistant_email.png)
![Seven Targets State](../../images/salesforce_seven_targets_state.png)
![Seven Targets Sequence](../../images/salesforce_seven_targets_sequence.png)

### Add trigger to the Lead Object in Salesforce
1. In _Lead_ Object go to _Triggers_ > Click on _New_ button to create new Trigger called LeadTriggerFor7Targets. Copy the code from [here](https://github.com/7targets/Salesforce-Integration/blob/main/LeadTrigger.tgr) to create a new trigger and then save the trigger. 

### Create Apex class to communicate with 7Targets
1. In _Setup_ search for _Apex Classes_ & create a new Apex Class called SevenTargetsLeadIntegration. You can find the code [here](https://github.com/7targets/Salesforce-Integration/blob/main/SevenTargetsLeadIntegration.cls). Copy and paste this code for this Apex class. 

#### Below details are required for the Apex class code to call the 7Targets APIs.
Get 7Targets API Client Id & Client Secret from support@7targets.com.  
1. Goto _Setup_ > search _custom metadata_ in Quick Find Box.
1. In _Custom Metadata_ create a new metadata named **7Targets API Credential** as shown below.
![7Targets API Credential](../../images/salesforce_seven_targets_api.png)
1. Add below fields in this Custom metadata.

| Field Label  | Field Name | Data Type |
| -------- | ------- | ------- |
| 7Targets Client Id  | Seven_Targets_Client_Id__c | Text Area(255) |
| 7Targets Client Secret | Seven_Targets_Client_Secret__c | Text Area(255) |
| 7Targets User ID  | Seven_Targets_User_ID__c	 | Text(100) |

### Create Connected App in Salesforce
1. If you don't have existing Certificate & Private Key then generate one from [here](https://developer.salesforce.com/docs/atlas.en-us.246.0.sfdx_dev.meta/sfdx_dev/sfdx_dev_auth_key_and_cert.htm?_ga=2.43114208.439795187.1656333652-1742453021.1655933163).
1. Create a Connected App in Salesforce using steps given [here](https://help.salesforce.com/s/articleView?id=sf.task_create_connected_app.htm&type=5). Copy Consumer key given which will be used in further setup.

## Configure 7Targets
1. In 7targets go to the _CRM_ page using menu bar from left side.
1. Add username(in the form of email), consumer key and private key(base64 Encoded [How?](#how-to-get-the-base64-encoded-string-for-private-key)). 
1. Use the Test button to verify that the provided credentials are working. 
1. Get the Assistant email and the sequence names by clicking on the respective buttons. Copy and Paste them in the relevant fields in the custom fields created for the Lead Object in Salesforce.

### How to get the Base64 encoded string for private key
> Private key create while creating the connected app, mostly is in the form of a file named **server.key**  
> Copy the content of that file and use https://www.base64encode.org/ to encoded that file content to Base64. Use that when creating/configuring 7Targets.

For any help feel free to drop us an email at support@7targets.com
