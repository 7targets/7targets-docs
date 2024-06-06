---
date: 2020-02-11
title: Whatsapp Message
description: Sending Whatsapp Message
type: Document
sidebar:
  - {id: create-provider, text: Create Provider}
categories:
  - manage-org
---

Following steps are valid assuming you have an existing Sinch account using which you want to send Whatsapp Messages from 7Targets

## Create Provider
Go to Whatsapp Settings page and Click on Add Provider button.
We currently only support Sinch as Whatsapp Provider.

You can get value for username, password & project Id from Sinch & value for client-id will be ipmessaging-client for Sinch.

Make sure you are marking checkbox at bottom is Default since in case of multiple providers default provider will be used.

![Whatsapp Provider](../../images/whatsapp_provider_info.png)

## Whatsapp Messages / Templates
After you have created a template in Sinch Dashboard you have to create same template in 7Targets

You can follow steps from [here](../../manage-org/organization-custom-message#whatsapp-message) to create Whatsapp Messages in 7Targets

## Using Whatsapp Message

**Add Leads :**
You can select Sequence containing Whatsapp Messages During Multiple Leads Upload You have also option of selecting Whatsapp Message Provider.

**Broadcast Whatsapp Message :**
To Broadcast a Whatsapp Message You have to select leads from Lead List & from _More Actions_ dropdown at the top of the Lead list select _Whatsapp Message_ option.

Create a new Broadcast By giving appropriate name, Broadcasting Date, select a Whatsapp Message from shown options & Click on Start Broadcasting button.