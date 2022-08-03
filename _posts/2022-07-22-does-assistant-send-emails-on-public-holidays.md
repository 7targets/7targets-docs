---
date: 2022-04-15
title: Does Assistant send emails on public holiday
# video_id: 6xyI5NNCCmc
description: Assistants tries to identify the leads country and avoid sending emails on public holidays. Off course you can overwrite this behaviour via the Assistant preference.

type: How-to
sidebar:
  - {id: step-1, text: Preference Do not send emails on holidays }
  - {id: step-2, text: How location of lead is known }

categories:
  - How-To
# set: getting-started
# set_order: 3
---
By default, Assistant does not send email to lead on lead's public holidays.

Based on the lead location, the Assistant tries to identify public holidays and does not send an email on those dates. E.g., if the lead is from the US then 4th of July is a public holiday and the Assistant will not send an email on that date.

You can overwrite this behaviour by changing the preference value

## Step-1
After going to that Assistant specific preference. Search for this specific preference by typing **holiday**.   
You will see something like the below image. Check or un-check the preference and save as per your requirement.

![image](../../images/preference-send-email-on-holidays.png)

## Step-2
How does Assistant get to know about the leads location. While uploading/adding the leads you can provide the location in the excel under a column with heading as **location**. 
If not provided, then Assistant tries to derive the location later when lead opens the email. 

If you have any further doubts, you can directly mail us at support@7targets.com.

