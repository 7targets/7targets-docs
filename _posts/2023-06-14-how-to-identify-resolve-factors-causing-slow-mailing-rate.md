---
date: 2023-02-08
title: How can I identify and resolve the factors causing a slow mailing rate?
# video_id: 6xyI5NNCCmc
description:  If you have been experiencing slow mailing rates and delays in email delivery, it's essential to understand the reasons behind this issue. This how-to guide will provide insights and steps to address the slow mailing rate and improve email delivery speed.
type: How-to
#sidebar:


categories:
  - How-To
# set: getting-started
# set_order: 3
---
Answer:
The rate of mailing can be slow at times due to several factors related to bounce rates and account management. Here's an explanation of why the rate of mailing may be slow:

1. Bounce Rate Monitoring: The Assistant regularly monitors the bounce rate based on the data from the last 15 days. If the bounce rate is below the specified pause limit (e.g., 5%), the Assistant takes a calculated risk and forcefully sends emails to a few leads with a "Pending" status. This is done to maintain a balance between valid email sends and unverified email addresses.
 [https://7targets.ai/help/how-to/how-to-calculate-bounce-rate/](https://7targets.ai/help/how-to/how-to-calculate-bounce-rate/)

2. Bounce Rate Threshold: When the bounce rate exceeds the specified pause limit (e.g., 5%), the account is automatically paused to prevent further issues. This pause is in line with the limits set by the AWS (Amazon Web Services) service used for email sending.
[https://7targets.ai/help/how-to/how-to-find-out-when-bounce-will-go-down/](https://7targets.ai/help/how-to/how-to-find-out-when-bounce-will-go-down/)

3. Account Management: The Assistant automatically manages the mailing process to ensure a balance between sending emails to verified email addresses and avoiding sending emails to unverified email addresses. This helps to maintain the bounce rate within acceptable limits and reduces the chances of being flagged for sending emails to invalid addresses.

4. Delay for Unverified Email Addresses: To prevent high bounce rates, unverified email addresses are intentionally delayed in the mailing process. This delay is based on the delivery of emails to verified addresses, ensuring that the bounce rate remains below the specified threshold.

5. Force Send Option: If you are certain that an email address is valid, you can use the "Force Send" option to bypass the delay for unverified email addresses. However, it's important to exercise caution when using this option, as sending emails to unverified addresses may result in a higher bounce rate.

6. Account Blocking: In cases where force sending backfires or if there are consistent issues with bounce rates, the account may be temporarily blocked for a period of 10-15 days. This is done to mitigate potential risks and maintain a healthy email sending reputation.

By managing the bounce rate and account status, the Assistant aims to prioritize valid email sends and minimize the risk of sending emails to unverified or invalid email addresses. It is important to follow the recommended procedures to ensure successful and efficient email delivery while maintaining a healthy email sending reputation.
