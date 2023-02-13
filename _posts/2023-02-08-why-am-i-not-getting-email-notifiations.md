---
date: 2023-02-08
title: Why am I not getting email notifications for response received ?
# video_id: 6xyI5NNCCmc
description: Why am I not getting email notifications for response received 
type: How-to
# sidebar:

categories:
  - How-To
# set: getting-started
# set_order: 3
---
Below are the possible reasons:
- notification may be disabled for the assistant
- email address in `Copy To` may not be correct and notification email sent bounced
- user email address is no more valid (user left the company). In this case, Assistant receives a bounce when tries to send the notification, then Assistant disables all the notifications to the user. Even if you enable the notification again from the UI, on the next notification it will bounce again and the notification will be disabled again. Read [how to handle user leaving company scenario]({{ site.baseurl }}/other/FAQ/#what-should-be-done-when-a-user-leave-an-organisation-)