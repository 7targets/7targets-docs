---
date: 2023-08-01
title: How to engage product users at various stages of user journey
description:  Engaging with users at different stages of their journey is crucial to ensure they get the most out of your product or service. Whether you have a SaaS solution or any other offering, leveraging 7Targets AI Assistant can greatly enhance user engagement.
#video_id: TcibhmCn9gM
type: How-to

sidebar:
  - {id: step-1-define-user-journey-stages, text: Define user journey}
  - {id: step-2-choose-an-approach---manual-or-automated, text: Choose an approach}
  - {id: manual-approach, text: Manual approach}
  - {id: automation-approach, text: Automation approach}
    - {id: conclusion, text: Conclusion}
categories:
  - How-To
# set: getting-started
# set_order: 3
---
Engaging with users at different stages of their journey is crucial to ensure they get the most out of your product or service. Whether you have a SaaS solution or any other offering, leveraging 7Targets AI Assistant can greatly enhance user engagement. We, at 7Targets, use this approach for our own customers and find it highly effective. Here's how you can do it:

## Step 1: Define User Journey Stages
The first step is to identify the various stages of your user journey. These stages represent different milestones or interactions that users go through while using your product or service. 

For instance, at 7Targets, we have the following stages:

| Sequence Name | Stage | 
|:--------|:-------|
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

## Step 2: Choose an Approach - Manual or Automated
Now, you have two options for implementing user engagement based on the defined stages: manual and automated.

Both approaches are useful. And have different costs. 

## Manual Approach:
In the manual approach, you use lead tags and sequences in 7Targets to organize and engage users. Create a unique tag for each stage you defined earlier. For example, the "User signed up" stage can be represented by the "SignedUpAssistantNotCreated" tag.

* Tagging Leads: Tag all leads in a specific stage with the corresponding tag. This will help you easily filter and categorize leads in your lead list.
* Assigning Sequences: Assign leads to the relevant sequences based on their tags. Each sequence represents a specific stage of the user journey.
* Transitioning Leads: As a lead progresses to the next stage, edit their tags accordingly. Remove the previous stage's tag and add the tag corresponding to the new stage. Then put the lead on the next sequence, ensuring they receive targeted engagement messages.

## Automation Approach:
In the automated approach, you can leverage APIs to seamlessly integrate with your system or software. Identify the user's stage in your system and use POST or PUT REST API calls to trigger the appropriate sequence in 7Targets.

* API Integration: Utilize the 7Targets [APIs](../../integrate/api/) to trigger the relevant sequence in response to the user's journey stage identified by your system.
* Utilizing Existing Sequences: Since you have predefined sequences in 7Targets for each stage, simply use the API to associate leads with the appropriate sequences.

## Conclusion:
Engaging users at different stages of their journey is essential for driving adoption and satisfaction. By using 7Targets AI Assistant and following the manual or automated approach, you can effectively engage users and provide a personalized experience based on their progression through the user journey.

For further assistance or more details, don't hesitate to contact our support team at support@7targets.com. We are here to help you make the most of your user engagement efforts.
