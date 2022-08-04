---
date: 2022-08-02
title: Why less emails than per day limit of the Assistant are sent
# video_id: 6xyI5NNCCmc
description: Sometimes Assistant sends less emails that the per day limit. Especially just after the leads are added.

type: How-to
sidebar:
  - {id: step-1, text: Schedule date is set when adding leads }
  - {id: step-2, text: Email id is validated when first email is to be sent }

categories:
  - How-To
# set: getting-started
# set_order: 3
---
Sometimes Assistant sends less emails that the per day limit. Especially just after the leads are added. 

Though this may seem like a problem, soon (just after all the first emails of leads are tried) assistant will send as per the per day limit. 

So nothing to worry actually.

## Step-1
When the excel file with leads are uploaded. Assistant distributes the leads (i.e. schedule the first email) as per the Assistant per day email sending capacity. 

So if the email sending capacity per day is 50 and 200 leads are uploaded, then assistant will schedule 100 leads for 2 different days. Assistant does double the capacity per day, because some email ids may not be valid. 

If invalid email ids are much more and the emails sent on that day are less than the limit, no problem within few days when the 2nd emails goes the capacity will be properly used. 

![image](../../images/lead-distribution.jpeg)

## Step-2
On the Day1 when the emails are to be sent, the email ids are validated and then the emails are sent. 

If more email ids are valid than the capacity then rest of the leads would be moved to the next available date. 

On Day 2, when the next set of leads are to be sent and if that is the first email then the email id is validated. If less than the capacity emails are valids then emails to those will go but it is balance out soon to use the complete capacity based on the schedule and the available capacity for the next day as per schedule. 

If you have any further doubts, you can directly mail us at support@7targets.com.

