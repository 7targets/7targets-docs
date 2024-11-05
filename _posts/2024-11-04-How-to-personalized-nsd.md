---
date: 2024-11-04
title: How do I schedule different Leads to send emails on different date ?
# video_id: ????????
description: When you want to schedule emails to go on pre-determined date for individual leads so that all leads won't be scheduled on single day.
type: How-to
sidebar:
  - {id: sending-emails-on-different-date, text: Send Emails on Different Dates }
categories:
  - How-To
---

## Sending Emails on Different Date
When scheduling emails for individual leads, you can ensure that each lead receives a reminder at a different date based on their unique needs. To achieve this, you will need to include a column named **Start Email Sending Date** in your data.

This column allows you to specify the exact date on which the first message will be sent for each lead. You can use this feature to nurture leads by sending them emails at strategic times.

To add the **Start Email Sending Date** column, follow these steps:

1. First, create a new column with this name in your existing data.
2. In this column, enter the specific date on which you want the first email to be sent for each lead.

![Example of the Start Email Sending Date column](../../images/Personalized_NSD.png)

**Uploading Data**

When uploading your data, you can also select the time at which the message will be sent on a specific date. This allows you to fine-tune the scheduling process and ensure that emails are delivered at the optimal time for each lead.

To do this, follow these steps:

1. On the Add Lead page, select the Time option.
2. Choose the date and time at which the first message will be sent.

![Example of selecting a date and time](../../images/date_Picker.png)

**Fallback Dates**

If any rows in the **Start Email Sending Date** column are empty, the system will use the date selected on the Add Lead page as a fallback. This is because sometimes data may not be complete, and using this fallback date ensures that emails are still sent at a strategic time.

By including the **Start Email Sending Date** column and utilizing this feature, you can schedule emails for individual leads to go out on different dates based on their unique needs. This allows you to nurture leads effectively and ensure that they receive reminders at optimal times.
