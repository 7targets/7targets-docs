---
date: 2022-04-12
title: Why do we seeing less link clicks in 7Targets email and more in google analytics
# video_id: 6xyI5NNCCmc
description: There are several reasons why we see inconsistencies in 7Targets link click report and google analytics reports.
type: How-to
sidebar:
  - {id: step-1, text: Phishing is rampant now}
  - {id: step-2, text: 7Targets ignore clicks in first 180 seconds}
  - {id: step-3, text: Webmail and ways of stopping read receipts}
  - {id: step-4, text: Seasonal google analytics shows higher visitors at times}
  - {id: step-4, text: Linkedin Ads}

categories:
  - How-To
# set: getting-started
# set_order: 3
---

There are several reasons for inconsistencies in 7Targets link click report and google analytics reports. Below are some of them: 

## Step-1
Phishing is rampant now, and many enterprises have added bots to their arsenal to check phishing links. 
Some bots provide a link click notification - even when a human is not reading it. 
Some bots do not provide a link click notification, as expected. 

## Step-2
7Targets Assistants ignore all clicks in first 180 seconds, assuming that humans do not click on links immediately after getting an email. This is a heuristic, and not a 100% perfect approach. 

We have seen some bots that kick in as late as after 10 minutes of sending email.
We have seen some humans click on emails immediately as well. 

## Step-3
**Webmail**: Default webmail settings do not allow read receipts. Webmail is launched in browsers, and browsers are more strict in default privacy and access settings. Normal email clients allow read receipts to be sent by default. 

**IT Admin**: Large companies, who have dedicated IT security/privacy personnel, who are paranoid of email configurations, can configure emails to not send read receipts across the org. They also add confidentiality disclaimers for all outgoing emails as well. Such companies usually hide read receipts. This also differs site to site of same company, based on which companies they acquired and how vigilant the IT was on these configurations. 

## Step-4
Once a month, you will also see google analytics show significantly higher visitors when you have done nothing different. These are web crawling search bots that are visiting your pages monthly to update their search engines. They are not from email sources. 

## Step-5
Linkedin Ads: Although LinkedIn has a disclaimer that 'bot clicks are not considered by LinkedIn algorithms while charging customers', bots have become smarter and we see link clicks from irrelevant sources from LinkedIn Ads as well. Although companies like LinkedIn and google analytics have teams on this problem of constantly removing bot sources, its not 100% accurate. 

These are some of the reasons why you will see difference in google analytics numbers and 7Targets dashboard numbers.

