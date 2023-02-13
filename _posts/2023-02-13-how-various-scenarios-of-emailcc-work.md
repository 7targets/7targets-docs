---
date: 2023-02-13
title: How does various scenarios of EmailCC work
# video_id: 6xyI5NNCCmc
description: EmailCC has various scenarios and understanding them in details will help use this simple and valuable functionality really well.
type: How-to
sidebar:
  - {id: create-lead-using-emailcc, text: Create Lead using EmailCC }
  - {id: acknowledgment, text: Acknowledgment } 
  - {id: actions-from-acknowledgment-email, text: Actions from Acknowledgment email } 
  - {id: response, text: Response } 
  - {id: user-replies, text: User replies } 
  - {id: no-response-from-lead, text: No response from Lead } 

categories:
  - How-To
# set: getting-started
# set_order: 3
---
EmailCC has various scenarios and understanding them in details will help use this simple and valuable functionality really well.

## Create Lead using EmailCC
Lead would be created by EmailCC when the user sends an email to someone and copies her/his Assistant. The default sequence for EmailCC would be used for this lead. 

![image](../../images/emailcc-1.jpg)

1. Lead would not be created by emailcc if a user who cc'ed is **NOT** a user in 7Targets. 
1. Lead would be created if the user who is cc'ing is an org admin in 7Targets. Irrespective of whether he was assigned to the assistant being copied or not.

## Acknowledgment
On creation of the lead from EmailCC, Assistant would send an email to the user with details of the schedule that the assistant will use, as well the name identified by the lead. 

How does the Assistant decide the name for this lead ? [Read here](../../getting-responses/assistant-details/#lead-name-for-emailcc)
![image](../../images/default-name.jpg)

If the user who cc'ed the assistant is not allowed to use the assistant, but is a valid user in 7Targets, then the user would get an email that says 'Right now you are not allowed to use assistant `<Assistant name>`. 
Enable EmailCC using these steps. And then cc the assistant again. Contact Org admin to assign assistant `<Assistant name>` to you.

Someone is not a user in 7Targets has cc'ed an assistant then she/he would not get any reply.

## Actions from Acknowledgment email
One important purpose of the Acknowledgment email from the Assistant is to inform the user about name, schedule, etc. Uaer would be able to easily take below actions.
![image](../../images/emailcc-ack-email.jpg)

1. Change the Lead Name
1. Verify that the Sequence is as expected
1. Change the Sequence

## Response
If Lead replies to the email from the user or Assistant, then the followup email sequence is stopped. Lead will not get any further emails from the Assistant. 

User would also get the Notification(Email and Whatsapp as per the preference) of this response from the Lead. 

If user does not reply in 24 hours of the response from Lead then `Lead is marked at risk email`(LAR - Lead at Risk). User would get notification about this.
LAR email notification go every 3 days to the user, till the user takes care of marks that lead is not at risk.

Once user replies, for a lead in LAR, LAR is removed automatically.

![image](../../images/lar.jpg)

## User replies
User replies back to the lead within 24 hours. Does the assistant followup again? 

User is responding from his email address and NOT from 7Targets. User gets a email directly from lead, because user had emailed the lead directly. Assistant was just in cc. 

`When user sends a reply, does assistant again tell the user within 5 minutes what is she going to do and how is she going to followup if a sequence was changed?`

After user replied back to lead from his email address, this reply email from the user would be saved in the timeline. If there are more followup emails to go (i.e. lead is in active followup sequence) then no change is done. But if no more followup emails are scheduled then the lead is restarted and put on the default emailcc sequence and user is notified too. 
![image](../../images/existing-lead-restart-preference.png)

## No response from Lead
Lead does not reply back and all followups are done. Then the Lead created via EmailCC is marked as LAR. And LAR notification to the user activates. This is done especially for leads created via EmailCC. 

If assistant preferences are set to change lead to 'Long term nurturing' after all followups are done. Then the leads goes to long term nurturing sequence and user is made aware of this.

![image](../../images/long-term-nurturing-preference.png)


If you have any further doubts, you can directly mail us at support@7targets.com.

