---
date: 2022-04-11
title: How Assistant can followup the campaign responses automatically
# video_id: 6xyI5NNCCmc
description: Responses and especially enquiries from a marketing campaign should not be dropped and possibly immediately responded with proper followup. AI Sales Assistant make that possible now.
type: How-to
sidebar:
  - {id: step-1, text: Enable the feature for the Assistant}
  - {id: step-2, text: Set campaign email id}
  - {id: step-3, text: Set Assistant email id for the campaign}
  - {id: step-4, text: Set assistant behavior, how do you want the assistant to respond}
  - {id: step-4, text: Tell the assistant what to do if its not a valid enquiry}

categories:
  - How-To
# set: getting-started
# set_order: 3
---
Many sales and marketing teams use bulk emailing for some campaigns. Especially when they havent yet identified thier ideal customer profile. Since this can blacklist their main domain, marketeers create a different domain from which this bulk email is carried out. Whenever someone responds, they provide a different 'Respond To' email address. 
Such 'Respond To' email boxes need to be monitored often. Most times good enquiries need immediate attention. Not doing so can result in lead getting dropped too. 

The goal is to respond fast to good enquiries and convert it into a meeting with the Sales Executive.

What happens most of the times is that such email boxes are forgotten for days. Many responses are not looked into immediately. And this is where 7Targets Assistants come in... 

7Targets allows you to assign responses from email campaigns as a lead directly to an Assistant. Assistant will do the following:
1. Read the email and Create a lead
2. Classify the response appropriately. For eg. Seeking more info, Hot, Deactivated, Unsubscribed, etc.
3. If the response is an Enquiry (Seeking more info) then the assistant assigns another email sequence to the lead immediately. 

How to setup this flow?

Its 5 simple steps. 

## Step-1
First, Enable this feature for the selected Assistant(s). Drop an email to support@7targets.com, provide your 7Targets user email along with the assistant name(s), and our support team will enable this feature for you. 

## Step-2
Mention the email address from where this campaign is run. Add multiple email ids if you are running multiple campaigns from different email boxes. 

## Step-3
Ensure that set the Reply-To attribute for your campaign emails to the Assistant's email id. So that the reply can be received by the Assistant and processed appropriately. 

Today, this is supported for Assistants that have Google Suite email ids. Refer [this]({{ site.baseurl }}/getting-started/create-your-assistant/#use-gmail) to create an Assistant using your existing GSuite email id. If you would like to support it for other email providers, please email support@7Targets.com.

![image](../../images/preference-for-emails-used-for-campaign.png)

## Step-4
Create a specific sequence where the first email is a quick 'Thank you' note with a link to book a meeting. Sequence can have a few more followup emails as well. 

If the lead respond backs to the followup emails then Assistant will invoke this sequence as a response. To avoid circular emailing, Assistant ensures that the same lead is NOT added to the same sequence if the lead responds back again.  

![image](../../images/preference-for-schedule-for-enquiry.png)

## Step-5
What happens is the response is not an enquiry? How the assistant classifies the flow in such cases? This is explained in below flow diagram. If the response is classified as something other than a Enquiry (Seeking more info) then what happens.

![image](../../images/how-does-campaign-response-lead-works.jpg)

If you have any further doubts, feel free to mail us at support@7targets.com.

