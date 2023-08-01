---
date: 2023-08-01
title: How to engage product users at various stages of user journey
description:  Your product, service or solution (SaaS or otherwise) would have users. These users would need to be engaged with to help them help them use your product well. 7Targets AI Assistant can be used for this. 
#video_id: TcibhmCn9gM
type: How-to

sidebar:
  - {id: decide-the-user-stages, text: Decide the user stages}
  - {id: two-ways, text: Two ways}
  - {id: manual, text: Manual}
  - {id: automation, text: Automation}
categories:
  - How-To
# set: getting-started
# set_order: 3
---
Your product, service or solution (SaaS or otherwise) would have users. These users would need to be engaged with to help them help them use your product well. 7Targets AI Assistant can be used for this. 
7Targets itself uses it for our own customers. 

## Decide the user stages
First thing to do is to decide the right user stages and write it down. 
For e.g. for 7Targets, we have below stages.

| Sequence Name | Stage |
| -------- | ------- |
| SignedUpAssistantNotCreated | Signed up and Assistant not yet created |
| AssistantCreated | User created Assistant successfully |
| LessThan10LeadsAdded | Less than 10 leads Added |
| LessThan25LeadsAdded | Less than 25 leads Added |
| LessThan100LeadsAdded | Less than 100 leads Added |
| MoreThan100LeadsAdded | More than 100 leads Added |
| TrialEndingIn2Days | Trial Ending in Two Days |
| LastDayOfTrial| Today is the Last Day of Trial |
| TrialEnded | Trial Ended |
| PlanActive | Your AI Sales Assistant Plan is Activated |

Once you have defined the user journey stages, then you can follow the details below to do it. 

## Two ways
First thing is to create a new Assistant specific for this purpose. With right title and signature, as well specific Nurturing table with right references and links. 

There are 2 ways to implement this using different 7Targets sequences: 
1. Manual
2. Automated 

Both approaches are useful. And have different costs. 

## Manual
Manally, it can be achived using lead `tags and sequences` in 7Targets.
Create tag for each of the stage already decided. Tag all leads in a given stage with that tag. Eg. User signed up stage can be represented with SignedUpAssistantNotCreated tag. 
- Putting right tags and removing the earlier stage tags will give a simple mechanism for you to filter the leads from the lead list

Now, you can filter the leads and put them on corresponding sequence as per tags.

When the lead moves to next stage, then edit the tags. Remove the earlier stage tag and add the new tag. Then put that lead (one or multiple) on the new sequence. 
And this will put this person on next sequence as per the stage. 

## Automation 
Instead of manually putting the person on a sequence as per stage, you will have to use [APIs](../../integrate/api/) from within your sytem. You can identify the stage in your system/software and make the right POST or PUT REST API calls. 

You already have the sequence in 7Targets as per the stage, which you can use in the API call. 

Feel free to reach out to us at support@7targets.com in case you need more details or any help.