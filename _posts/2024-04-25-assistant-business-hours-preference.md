---
date: 2024-04-25
title: How assistant business hours preference works
#video_id: JC2yJnBXzLM
description: Sending Follwups only during business hours
type: How-to
sidebar:
  - {id: setting-business-hours, text: Setting Business Hours}

categories:
  - How-To
# set: getting-started
# set_order: 3
---
## Overview
7Targets AI assistant works around the clock to send followup using scheduled date till it's daily limit is reached. But Sometimes you only want to send followups during certain time such that lead can immediately read & respond to those followups.

To send followups during desired timing you can set a time range only during which followups will be sent.

You can set this preference using following steps

1. Go to Assistant Preference from left side bar
2. Select an assistant for which you want to set Business Hours
3. Select Desired Timezone
3. Add Start and End time preference for Time Range as shown below.

![Business Hour Preference](../../images/business_hours_preference.png)

Now Assistant will only send further followups during time range defined by Start Time and End Time.

If a user adds scheduled date which is out of give business hours then it will show a warning as shown below

![Business Hour Warning](../../images/business_hour_warning.md)

### Exceptions to business Hours
Business hour preference doesn't apply in following cases:
- ![Send Time Optimization](./2023-06-14-what-is-send-time-optimisation.md)
- ![Processing Pending Leads](./2023-02-09-how-are-pending-leads-processed.md)
- Overriding business hours by adding Scheduled date outside given range.

#### Override Business Hours**
You have the flexibility to override the start hour of your business hours based on your preferences. If your business hours are set from 9:00 AM to 7:30 PM, but you prefer follow-ups to begin later in the day for particular lead file, you can specify a different scheduled time, such as 3:00 PM while adding leads. This means that follow-ups will start at 3:00 PM and continue until the end of your regular business hours at 7:30 PM.

How it Works:

- **Standard Business Hours :** By default, your business hours are set from 9:00 AM to 7:30 PM.
- **Custom Start Time :** If you choose a scheduled time, such as 3:00 PM, it will override the standard start time of 9:00 AM.
- **Consecutive Days :** This adjustment applies to all consecutive days. Follow-ups will consistently occur between the specified start time and the regular end time.

This flexibility allows you to tailor your business hours to better suit your workflow and preferences.