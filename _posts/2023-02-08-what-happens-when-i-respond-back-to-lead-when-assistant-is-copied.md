---
date: 2023-02-08
title: What happens when I respond back to lead and assistant is copied ?
# video_id: 6xyI5NNCCmc
description: When you (user) reply back to the lead copying Assistant, it is like letting the Assistant know that you have taken care, so do not put the lead at risk.
type: How-to
sidebar:
  - {id: scenario-1, text: Scenario 1 }
  - {id: scenario-2, text: Scenario 2 }

categories:
  - How-To
# set: getting-started
# set_order: 3
---
When you (user) reply back to the lead copying Assistant, it is like letting the Assistant know that you have taken care, so do not put the lead at risk. If lead is already at risk then take it out of risk.

Assistant needs to differentiate above with a request to followup the lead (EmailCC). So there are two scenarios:
## Scenario 1
If you are replying to an email which has the one of the emails sent by the Assistant at the bottom, then Assistant would be able to identify this as not to be considered for EmailCC, but just as a reply to lead. In that case Assistant would take out the lead from at risk (if it is at risk) and would not send any reminder emails to you.
## Scenario 2
If you are replying to an email which **does not** have any email from Assistant. e.g. you sent an email to the lead and copied the assistant (for EmailCc). Lead then responds to this email and Assistant is copied in that too. Then you reply to this email from lead. In this case, Assistant has not sent any email to lead. In such a scenario, Assistant would consider as EmailCc and would restart the lead for followup.