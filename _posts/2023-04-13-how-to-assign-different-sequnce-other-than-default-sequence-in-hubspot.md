---
date: 2023-03-31
title: How do I assign some other 7Targets sequence to the contacts in Hubspot ?
# video_id: 6xyI5NNCCmc
description:  7Targets Assistant has a default sequence. And when assigning the contact to the assistnat in Hubspot the default sequence would be picked up. But sometime you want some other sequence to be used instead of default sequence of Assisant. You can do this by following below steps.
type: How-to
#sidebar:

categories:
  - How-To
# set: getting-started
# set_order: 3
---

7Targets Assistant has a default sequence. And when assigning the contact to the assistnat in Hubspot the default sequence would be picked up. But sometime you want some other sequence to be used instead of default sequence of Assisant. You can do this by following below steps:

## 1. Edit the 7Targets sequence:
Edit the 7Targets sequence in the field `7Targets Sequence`. If you do not see all the Sequences in the drop down list then you have to go to 7Targets Org Messges->CRM and click on "Sync Sequence".
![image](../../images/case1_2.png)

This is for one contact and same can be done for multiple contacts too.

## 2. Now assign to Assistant:
Now assign the contact to the Assistant. This will get the 7Targets Assistant started with the sequence provided in the above step. If no seuence is provided in the above step then the default sequence of the Assistant is picked up. 
![image](../../images/case1_3.png)

## 3. Verify the sequence in 7Targets:
Verify the sequence for these contacts/leads in 7Targets. Go to 7Targets, and there you can check the sequence of the particular lead is according to what you had specified in Step 1.
![image](../../images/case1_4.png)

You can do this for multiple contact at same time too. In Hubspot, on selecting multiple contacts change the 7Targets Sequence value using the Edit action before changing the owner to the Assistant. 

Important point to note for reassignment of Contact in Hubspot to Assistant, you have to change the 7Targets Sequence value to something else or delete the value else same Sequence will be picked up again. 
