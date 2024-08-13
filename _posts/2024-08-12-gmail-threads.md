---
date: 2024-08-13
title: Follow-up Emails Not Threading Together
description: Understanding why follow-up emails might not appear in a single thread when CCing an assistant.
type: Document
sidebar:
  - {id: why-followups-not-same-thread, text: Why Aren't My Follow-up Emails in the Same Thread?}
  - {id: causes-followup-thread-issue, text: What Causes This Issue?}
categories:
  - How-to
---

<a name="why-followups-not-same-thread"/>
## Why Aren't My Follow-up Emails in the Same Thread?

When you send an initial email using Gmail or Outlook and CC an assistant, the assistant takes over with follow-ups.  
Sometimes, these follow-ups might not appear in the same thread as the original email.

<a name="causes-followup-thread-issue"/>
## What Causes This Issue?

This usually happens because certain email headers, such as *In-Reply-To* and *References*, are missing.  
These headers are necessary for threading emails together.  
Google’s [blog post](https://workspaceupdates.googleblog.com/2019/03/threading-changes-in-gmail-conversation-view.html) explains that emails will not appear in the same thread unless these headers contain the previous email’s *Message-ID*.

7Targets includes these headers to ensure threading.  
However, different email client settings or filters may still cause emails to appear in separate threads.
