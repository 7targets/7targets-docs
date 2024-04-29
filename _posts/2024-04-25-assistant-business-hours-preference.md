---
date: 2024-04-25
title: How assistant business hours preference works
#video_id: JC2yJnBXzLM
description: Sending Follwups only during business hours
type: How-to
sidebar:
  - {id: overview, text: Setting Business Hours}
  - - {id: how-it-works, text: How it Works}

categories:
  - How-To
# set: getting-started
# set_order: 3
---
## Overview
7Targets AI assistant works around the clock to send followup using scheduled date till it's daily limit is reached.  
But Sometimes you only want to send followups during certain time of the day (Business Hours).

To send followups during desired timing you can set the business hours preference for the Assistants.

You can set this preference using following steps

1. Go to Assistant Preference from left side bar
2. Select an assistant for which you want to set Business Hours
3. Select Desired Timezone
4. Add Start and End time preference for Time Range as shown below.
5. You can copy this to all other assistants too.

![Business Hour Preference](../../images/business_hours_preference.png)

Now Assistant will send email only during time range defined by Start Time and End Time.

If a user adds scheduled date which is out of give business hours then it will show a warning as shown below.

![Business Hour Warning](../../images/business_hour_warning.md)

### Exceptions to business Hours
Business hour preference **doesn't** apply in following cases:
- ![Send Time Optimization](./2023-06-14-what-is-send-time-optimisation.md)
- ![Processing Pending Leads](./2023-02-09-how-are-pending-leads-processed.md)
- Overriding business hours by adding Scheduled date outside given range.
- Any automated email send as a response to asking for brochure will not consider the business hours

#### Override Business Hours**
You have the flexibility to override the the business hours preferences. If your business hours are set from 9:00 AM to 7:30 PM, but you prefer follow-ups to begin later in the day for particular lead file, you can specify a different scheduled time, such as 3:00 PM while adding leads. This means that follow-ups will start at 3:00 PM and continue until the end of your regular business hours at 7:30 PM.

## How it Works:

### Scenario 1: 
If your business hours are set from 9:00 AM to 7:30 PM, and while ading leads you provide a time as 3:00 PM. Then the follow-ups will start at 3:00 PM and continue until the end of your regular business hours at 7:30 PM. Leads beyond this time will be moved to next day 3:00 PM onwards

### Scenario 2: 
If your business hours are set from 9:00 AM to 7:30 PM, and while ading leads you provide a time as 8:30 PM. Then it is like you want to override the business hours, so your choice will be given priority and emails will go as per your choice. 
