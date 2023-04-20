---
date: 2023-03-31
title: What if the next email for the lead is going beyond the out of office date for the lead ?
# video_id: 6xyI5NNCCmc
description:  When out of office (OOO) reply is received from the lead, the AI assistant sends the next email after the Out of office date.
type: How-to
#sidebar:

categories:
  - How-To
# set: getting-started
# set_order: 3
---

## Out of office date usage
According to Out of Office classification, the Assistant should have sent the next email after the Out of office date, say 8th Nov, but why did Assistant still scheduled it for 16th Nov?

In the above scenario, the next scheduled date for the next email to be sent was already at 16th. The Lead was out of the office. Lead was returning on 8th of the same month. So no change of schedule date is done by the Assistant.

What happens if Out Of Office date is before the date when next email is scheduled?

In such a case, AI assistant will not change the Next Scheduled date. Assistant will continue to follow-up as per the already scheduled date.

`Note`: If the next email was scheduled on or before the date when the lead is out of office, in that case the AI assistant will not send an email, because Assistant can read and understand that the lead is not in office. Hence, the assistant will automatically shift the next email to go after the lead returns to office.

In this case above, if the next scheduled date was before 8th (when the lead was not in office), then AI assistant will automatically shift the email sending date to next business day.

## Questions answered
- When will the Assistant stop sending messages ? 