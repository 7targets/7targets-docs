---
date: 2020-01-13
title: Lead State and Responses
description: Lead Responses, Lead State and Teach your Assistant
type: Document
sidebar:
  - {id: lead-responses, text: Lead Responses}
  - {id: lead-state, text: Lead State}
  - {id: teach-your-assistant, text: Teach your Assistant}
  - {id: questions-answered, text: Questions answered}
categories:
  - assigning-leads
---

<a name="lead-responses"/>
## [Lead Responses](#lead-responses)
What will the Assistant do when a response is received?  
Emails responses are read by the Assistant and would try and decide the email intent.  

The machine learning model/s tries to identify the response to one of the below. 
- out of office or 
- asks to stops sending any further emails or 
- agrees to have a meeting at a particular day or
- requests for brochure  
- request to check back later
- unsubscribe me
 
This helps the assistant take right action and update the lead state.  
Some examples are mentioned below:

| Response | Inference | Action | 
|:-------|:--------|:--------|
| I am out of office for 2 weeks. If urgent ...  | Lead is Out of office.  | Connect when lead is back after 2 weeks  |
| I am not the right person. Please don't email me. | Wrong Lead | Stop further Communication |
| Please send me your brochure. | Warm Lead| Send the email with brochure immediately. Then stop further Communication |
| Send me your company profile. | Warm Lead| Send the email with brochure immediately. Then stop further Communication |
| Setup a meeting for tomorrow 5 PM | Hot Lead | Forward email thread to Sales. Notify Sales on Phone. Stop further Communication with the Lead. Remind sales after 24hrs to avoid this lead being dropped |
| We are busy in some other priorities right now. Lets talk sometime in Jan. | Warm Lead | Set future communication in Jan. |
| Unsubscribe me from your mailing list | Unsubscribed | Lead would be marked as unsubscribed. |

## [Lead State](#lead-state)
Assistant will categorize the leads in various states based on the followups and responses. Various possible state are:   
`New` conveys that the lead added cannot be processed as you have used up your leads limit as per the plan. You can Restart these leads in the next period or upgrade your plan and then restart these leads now.  
`Cold` the followup is under progress.   
`Hot` if the lead has accepted to meet.   
`Warm` lead is someone who has opened 3 or more emails. A good list for your calling team to call.  
`Engaged` lead is someone who has opened 1 or more emails.  
`Processed` followup is completed as per the schedule and there was no response from the lead.    
`Out of office` received an out of office from the lead. Assistant will restart the followup after lead returns back to office.  
`Deactivated` lead responded back asking to stop sending emails. Lead email id is invalid as verified by the assistant. Email sent to the lead bounced. 
`Unsubscribed` lead used the unsubscribed link in the email or responded asking to unsubscribe. You wont be able to send any more emails to this lead.  
`Responded` state for the lead conveys that there is some response from the lead and Assistant was not able to categorize it to one of the above.  
`Pending` means Assistant is still validating the email address of the lead.  

## Teach your Assistant
Some of the responses may over fit or under fit the out-of-the-box ML model and the response received from the lead may get identified in a State which may not be most correct.  
Some responses could be very specific to your industry and customer profile and so this may happen when out of the box ML model is used. 
  
**Assisted Learning** is the possible solution for above problem. You can provide specific terms from the response email and mention which sub_state and state it should be mapped to. This will be specific to your organisation, any response received will be passed through a rudimentary model created from this small amount of data.  
* If there is a match with more than 90% confidence then that assisted learning mapping would be used. 
* If more than one row matches with more than 90% confidence then the highest confidence mapping would be used.
* If no row with 90% or more confidence matches then anyways the out of box model in 7Targets would be used.

You would also see a note added mentioning which mapping was used from the Assisted Learning, if Assisted learning mapping is used.

## Questions answered
- Why some leads are showing as Pending ?
- Why some leads are showing as New ?
- Why some leads are showing Deactivated ?
- What will the Assistant do when a response is received ? 
- When will the Assistant stop sending messages ? 
