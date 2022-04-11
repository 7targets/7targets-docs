---
date: 2022-04-11
title: How Assistant can followup the campaign responses automatically
# video_id: 6xyI5NNCCmc
description: Responses and especially enquiries from a marketing campaign should not be dropped and possibly immediately responded with proper followup. AI Sales Assistant make that possible now.
type: How-to
sidebar:
  - {id: step-1, text: Enable the feature for the Assistant}
  - {id: step-2, text: Set preferences for email used for campaign}
  - {id: step-3, text: Set preference for schedule to use for enquiry}
  - {id: step-4, text: What happens if the response is not an Enquiry}

categories:
  - How-To
# set: getting-started
# set_order: 3
---
Some marketing and sales teams faced this problem of responses (more specifically enquiries) from the email campaign not getting immediate attention and at times getting dropped too. 

The email campaign was run from a different tool and team members were responsible to keep and eye on  responses. Understand the details and get back soon in case of enquiries. Knowing well that the goal is to provide the available info and try and get a meeting with Sales Executive.

Now, a feature in 7Targets allows one to assign this response from email campaign as a lead directly to the Assistant. Assistant will do below:
1. Create a lead
2. Classify the response into (Seeking more info, Hot, Deactivated, Unsubscribed, etc)
3. If the response is an Enquiry(Seeking more info) then put the lead on the schedule set in the preference. 

Below are the steps to use this feature. 

## Step-1
First, this feature has to be enabled for the Assistant/s. Drop an email to support@7targets.com providing your 7Targets user email and the assistant name and email, to enable this feature for those Assistants. 

## Step-2
To be able to classify the response from a campaign email correctly, it is important to set this preference. It conveys from which email ID the original campaign was sent out. You can put multiple email ids here so that you do not have to come and edit every time a new campaign is run. 

One important thing to note is to set the Reply-To attribute for your campaign emails to the Assistant's email id. So that the reply can be received by the Assistant and process it as expected. 

Today this is supported only for Assistant with email on Google Suite. Refer [this]({{ site.baseurl }}/getting-started/create-your-assistant/#use-gmail) to create an Assistant using your existing GSuite email id. 

![image](../../images/preference-for-emails-used-for-campaign.png)

## Step-3
You will have to create a specific schedule which possibly sends a quick Thank you note with a link to book a meeting. And may contain few followup emails too. 

If the lead respond backs to the followup emails then Assistant will process it as a response. Assistant will make sure to NOT put the lead back on same schedule if the next response is classified as Enquiry too. 

![image](../../images/preference-for-schedule-for-enquiry.png)

## Step-4
Below flow explains how does it work. And if the response is classified as something else than Enquiry (Seeking more info) then what happens.

![image](../../images/how-does-campaign-response-lead-works.jpg)

If you have any further doubts, you can directly mail us at support@7targets.com.

