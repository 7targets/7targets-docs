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
Deals from **Pipedrive** CRM can be assigned to 7Targets AI Sales Assistant directly within the Pipedrive UI. AI Assistant will then own the deal and communicate to try and get the meeting. Assistant will also update the deal by putting notes for the emails being sent.

One **important** point to note, as soon as the AI Assistant receives a response from the deal and detects it to be a Hot or Responded deal then the assistant assigns the deal back to the original owner.


## Authorize Pipedrive for 7Targets 
1. When you signup on 7Targets, an Assistant will be created for you.You can choose to use the same assistant or you can create a new assistant for Pipedrive. Provide the default values for context and other variables at the Assistant level by editing the Assistant. Make sure you Signup/Login on 7Targets before moving ahead. 

2. Signup/login on Pipedrive.

3. **Authorize Pipedrive** by clicking this link [authorize](https://solution.7targets.com/pipedrive-authorize){:target="_blank" rel="noopener"}. 
You will see the below page. Click on `Allow & Install`
![pipedrive 1](../../images/pipedrive_1.PNG)
Once Authorization is complete Click on `Click Here`. 
![pipedrive 2](../../images/pipedrive_2.PNG)

4. In 7Targets, under user profile, look at the "CRM Details" tab. Various status and the meanings are below:   
**ASSISTANT_EXISTS_AS_USER_IN_CRM** : You are all set. Go ahead and assign one contact from Pipedrive to the Assistant user in Pipedrive. That contact should be seen as deal in 7Targets in few seconds.  
**ASSISTANT_DOES_NOT_EXISTS_AS_USER_IN_CRM** : Follow step 2 and beyond above.  
**ASSISTANT_NOT_YET_CREATED** : Follow Step 1 onwards.  
**ALL_WORKING_WELL** : All set, it is working well for you.  
![pipedrive 3](../../images/pipedrive_3.PNG)

5. In Pipedrive, click on `+ Deal` option on Deals page. When the below popup opens up click on `Settings` as highlighted.
![pipedrive 4](../../images/pipedrive_4.PNG)

6. On the Settings page you can see the custom fields created. Thee fields are of 7targets and visible after successful Authorization.
![pipedrive 5](../../images/pipedrive_5.PNG)

7. Click on the custom fields and select the checkboxes as shown below.
![pipedrive 6](../../images/pipedrive_6.png)
![pipedrive 7](../../images/pipedrive_7.PNG)

8. Once above setps ar done, you can go ahead and add a Deal with Name, Organisation and Email fields etc. Do not assign any value in `7ts_assistant` and other custom fields of 7Targets while adding a deal.
![pipedrive 8](../../images/pipedrive_8.png)

9. Once deal is added, click on it and a deal page will open up.Here you can assign `7ts_assistant`and `7ts_schedule` and other 7ts fields.Once you assign values to these fields, a Lead will be created in 7Targets for the respective Deal in Pipedrive.
![pipedrive 9](../../images/pipedrive_9.png)

10. In 'Activities' tab of Pipedrive, you can the following message indicating that Lead has been added to 7Targets.
![pipedrive 10](../../images/pipedrive_10.PNG)

11. You can verify the same in 7Targets screen under 'Leads' tab.
![pipedrive 11](../../images/pipedrive_11.png)

12. If you intend to pass context to the lead from Pipedrive then use the custom field named "7Targets Context" for Deals in Pipedrive. With this, when you assign the deal to Assistant and if there is any context provided for this lead/deal then Assistant will use that else it will use the default context at the Assistant level in 7Targets.