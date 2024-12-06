---
date: 2020-02-11
title: SMS Message
description: Sending SMS Message
type: Document
sidebar:
  - {id: create-provider, text: Create Provider}
categories:
  - manage-org
---

Following steps are valid assuming you have an existing Twilio account using which you want to send SMS Messages from 7Targets

## Create Provider
Go to SMS Settings page and Click on Add Provider button.

We currently only support Twilio as SMS Provider.

You can get value for Sender Phone Number, Account SID & Auth Token from Twilio.

Make sure you are marking checkbox at bottom is Default since in case of multiple providers default provider will be used.

![SMS Provider](../../images/SMS_provider_info.png)

## SMS Messages / Templates
After you have created a template in Twilio Dashboard you have to create same template in 7Targets

You can follow steps from [here](../../manage-org/organization-custom-message#SMS-message) to create SMS Messages in 7Targets

## Using SMS Message

**Add Leads :**
You can select Sequence containing SMS Messages During Multiple Leads Upload. You have also option of selecting SMS Message Provider.

**Broadcast SMS Message :**
To Broadcast a SMS Message You have to select leads from Lead List & from _More Actions_ dropdown at the top of the Lead list select _SMS Message_ option.

Create a new Broadcast By giving appropriate name, Broadcasting Date, select a SMS Message from shown options & Click on Start Broadcasting button.