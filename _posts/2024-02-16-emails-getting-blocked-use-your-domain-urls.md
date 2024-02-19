---
date: 2024-02-12
title: Emails getting blocked? Use your own domain tracking urls
description: If the content of your email is deemed spammy because of some external domain links for tracking urls, then Gmail and Outlook may block your account, or your recipient's email servers may block your emails. 
#video_id: TcibhmCn9gM
type: How-to

sidebar:
  - {id: overview, text: Overview}
  - {id: your-emails-could-be-blocked, text: Your emails could be blocked}
  - {id: simple-solution, text: Simple solution}
  - {id: tracking-domain-details, text: Tracking domain details}
  - {id: additional-help-for-creating-the-tracking-domain, text: Additional help}
  
categories:
  - How-To
# set: getting-started
# set_order: 3
---

## Overview
7Targets doesn't keep an eye on its users from content perspective, so you can get started right away without waiting for approval. We rely on Google to handle most monitoring tasks. If you try to send spam using 7Targets, Google's systems will likely detect it and block your account. We trust Google's system; it's hard to imagine we could create a better one for catching spammers.

## Your emails could be blocked
Legitimate emails could get mixed up with a spammer's, leading to blocks. How does this happen? If you use 7Targets' tracking features like open tracking, click tracking, unsubscribe a "tracking domain" is added to your emails.  

For instance, if you use open tracking, a hidden pixel is placed in your emails with the tracking domain.  

Similarly, if you're tracking clicks, your links are modified to go through 7Targets' server via the tracking domain. 

If you haven't set up a custom tracking domain, 7Targets uses shared tracking domain. Some spam filters flag common spam domains. If your emails share the same tracking domain as spam emails, they might also get blocked.

## Simple solution
The solution is straightforward: Your accounts should have a tracking domain dedicated solely to your emails.

1. Lets create a SSL certificate for your domain. Drop an email to support@7targets.com 
1. Create CNAME records for your domain to create a branded tracking domain for your 7Targets Assistants using your OWN domain name. Take the CNAME record value from 7Targets support team 
1. Once above steps are done, copy the tracking url to the Assistants using Edit Assistant option. Screen shot below. 

This is the most crucial step you can take to boost your email deliverability and steer clear of blocking problems.

## Tracking domain details
![own tracking domain](../../images/own-tracking-domain-details.png)

## Additional help for creating the tracking domain

https://www.youtube.com/watch?v=Ytr7R_BN0JY   

https://www.youtube.com/watch?v=-GJ7IsVXuwA