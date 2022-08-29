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

## [What is Engaged, Warm and HOT leads?](#lead-state)
Assistant will categorize the leads in various states based on the followups and responses. Various possible state are:   
`New` conveys that the lead added cannot be processed as you have used up your leads limit as per the plan. You can Restart these leads in the next period or upgrade your plan and then restart these leads now.  
`Cold` the followup is under progress.   
`Hot` if the lead has accepted to meet.   
`Warm` lead is someone who has opened 3 or more emails or has clicked on a link from the email. A good list for your calling team to call.  
`Engaged` lead is someone who has opened 1 or more emails.  
`Processed` followup is completed as per the schedule and there was no response from the lead.    
`Out of office` received an out of office from the lead. Assistant will restart the followup after lead returns back to office. [What if the next email for the lead is going beyond the out of office date for the lead ?](./#out-of-office-date-usage)   
`Deactivated` lead responded back asking to stop sending emails. Lead email id is invalid as verified by the assistant. Email sent to the lead bounced.  
`Unsubscribed` lead used the unsubscribed link in the email or responded asking to unsubscribe. You wont be able to send any more emails to this lead.  
`Responded` state for the lead conveys that there is some response from the lead and Assistant was not able to categorize it to one of the above.  
`Pending` means the email id was NOT certain to be valid (Un-verifiable), so Assistant will process these leads at a slower rate to avoid getting into Bounce issues.  

## Teach your Assistant
Some of the responses may over fit or under fit the out-of-the-box ML model and the response received from the lead may get identified in a State which may not be most correct.  
Some responses could be very specific to your industry and customer profile and so this may happen when out of the box ML model is used. 
  
**Assisted Learning** is the possible solution for above problem. You can provide specific terms from the response email and mention which sub_state and state it should be mapped to. This will be specific to your organisation, any response received will be passed through a rudimentary model created from this small amount of data.  
* If there is a match with more than 90% confidence then that assisted learning mapping would be used. 
* If more than one row matches with more than 90% confidence then the highest confidence mapping would be used.
* If no row with 90% or more confidence matches then anyways the out of box model in 7Targets would be used.

You would also see a note added mentioning which mapping was used from the Assisted Learning, if Assisted learning mapping is used.

<a name="out-of-office-date-usage"/>
### [Out of office date usage](#out-of-office-date-usage)
According to Out of Office classification, the Assistant should have sent the next email after the Out of office date, say 8th Nov, but why did Assistant still scheduled it for 16th Nov?

In the above scenario, the next scheduled date for the next email to be sent was already at 16th. The Lead was out of the office. Lead was returning on 8th of the same month. So no change of schedule date is done by the Assistant.

What happens if Out Of Office date is before the date when next email is scheduled?

In such a case, AI assistant will not change the `Next Scheduled date`.  Assistant will continue to follow-up as per the already scheduled date.

Note: If the next email was scheduled on or before the date when the lead is out of office, in that case the AI assistant will not send an email, because Assistant can read and understand that the lead is not in office. Hence, the assistant will automatically shift the next email to go after the lead returns to office.

In this case above, if the next scheduled date was before 8th (when the lead was not in office), then AI assistant will automatically shift the email sending date to next business day.

## Questions answered
- Why some leads are showing as Pending ?
- Why some leads are showing as New ?
- Why some leads are showing Deactivated ?
- What will the Assistant do when a response is received ? 
- When will the Assistant stop sending messages ? 
