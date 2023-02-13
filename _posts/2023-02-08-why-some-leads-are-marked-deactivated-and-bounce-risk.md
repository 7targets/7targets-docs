 ---
date: 2023-02-08
title: Why some leads are marked Deactivated and Bounce Risk ? OR Why do I see a note like Bounce rate beyond limit and the email is not sent for the lead?
# video_id: 6xyI5NNCCmc
description:  Why some leads are marked Deactivated and Bounce Risk
type: How-to
# sidebar:

categories:
  - How-To
# set: getting-started
# set_order: 3
---
In the email ecosystem, it is critical to maintain a healthy Reputation.  
Bounced emails impacts the credibility of the email servers and reduces the deliverability of your emails.

If too many bad email ids come into the system, then email systems blocks that user beyond a particular bounce rate. The next thing a human has to do is wait for a few days and then retry the good email addresses. Thats what the AI Assistant does automatically.

To achieve the better deliverability for our customers, we have the bounce rate limit for each of our customers at the organization level. If the Bounce rate of 4% is hit then we do not take risk of sending emails to email ids which are verified as Risky to send.   
While, we continue to send emails to Email ids which are verified as Safe to send. 
We use multi-layer approach to validate the email ids before sending any emails.  

Bounce rate is calculated based on the number of Bounce Deactivated leads in the last 7 days compared to leads created. The Assistant continues to retry sending the email for the next 15 days while checking the bounce rate every day, hoping that it will go down in few days. While retrying, Assistant leaves a note `Cannot process as Bounce Rate is beyond the limit and email is not certain to be valid...` in the lead for the user to know what is happening. 

Even after trying for 15 days    
`IF` your Org level bounce rate is beyond the limit  
`THEN` those leads are marked Deactivated and Bounce Risk.