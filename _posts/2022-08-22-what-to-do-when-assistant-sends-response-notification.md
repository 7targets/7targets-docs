---
date: 2022-08-19
title: What to do on receiving Response Notification from Assistant
# video_id: 6xyI5NNCCmc
description: Assistant notifies the user on receiving a favourable response from the lead. So that user can act on it.  

type: How-to
sidebar:
  - {id: lead-list, text: Lead List }
  - {id: export-leads, text: Export Leads}
  - {id: valid-leads, text: Valid Leads}
  - {id: accidental-mistake, text: Accidental Mistake }

categories:
  - How-To
# set: getting-started
# set_order: 3
---
Assistant notifies the user on receiving a favourable response from the lead. So that user can act on it. 

User has multiple ways of handling this situation.
- Introduce yourself or someone in the team to take the discussion ahead. 
- Send email as Assistant

If user do not take care of the response in 24 hrs then lead is marked at risk and Assistant follows up with the lead owner, which the user can disable if the action is taken outside of the system.

## Lead List
On click of the Total Leads and Total Valid Leads count in the Dashboard, you would be shown total leads in the lead list for the filtered period. Default period is last 90 days. 

Select all the leads and then click on the Export icon. Provide the name and you will be informed on email when the export is complete. 
![image](../../images/export-leads.jpg)

## Export Leads
You can also click on the More and Exports to get to the page which shows the exported leads. 
![image](../../images/export-list.jpg)

And then Download the exported file. 
![image](../../images/export-list-download.jpg)

## Valid Leads
You can open the downloaded CSV in microsoft excel and apply the specific filters to get to your data. 

![image](../../images/export-csv.jpg)

Note below is the list of Sub-States which are considered as Invalid leads. You can filter out on those Sub-States in the file and get the list of valid leads.  
- **InvalidEmail** (Email was identified as Invalid when checked against the email validation solutions like debounce, zerobounce)
- **BounceDeactivated** (We received a bounce notification after an email was sent)
- **BounceRisk** (Email was identified as risky to send when checked against the email validation solutions like debounce, zerobounce)
- **CannotDetermine** (We received a bounce notification  after an email was sent, it did not contain enough information to know the reason)
- **ServerUnReachable** (Email validation solutions like debounce, zerobounce, was not able to reach the email server for the provided email)
- **SpamTrap** (Is a Spam Trap so not a valid email)
- **Disposable** (Is a disposable email, so not considered valid)

## Active Leads
A quick note about **Active Leads**.  
What are Active Leads?  
Why do at times the count on the dashboard and lead list count do not match for Active Leads ?  

Active Leads are leads, which are scheduled to receive an email in future. 
To get the active leads in the lead list, one has to use the **Scheduled** by date filter. And provide the future date in **to**. 
Based on the time period it will show the leads in the list. 

Dashboard is for past data, the default time period for Dashboard is past 90 days (Quarter).  
But, Active Leads are for future date, so when clicked on the Active Leads count in dashboard, by default we pick 180 days in future. 
If some leads are schedule beyond the **To** date, then the count may not match. You can simply increase the **To** date in the filter to get leads beyond the default time.

![image](../../images/schedule-date-filter.jpg)

If you have any further doubts, you can directly mail us at support@7targets.com.

