---
date: 2020-02-13
title: Custom Message 
description: Custom Message for Custom Sequence
# video_id: TcibhmCn9gM
type: Document
sidebar:
  - {id: custom-messages, text: Custom Messages}
  - {id: personalization, text: Personalization}
  - {id: image-in-email, text: Image in Email}
  - {id: whatsapp-message, text: Whatsapp Message}
  - {id: sms-message, text: SMS Message}
  - {id: questions-answered, text: Questions answered}
categories:
  - manage-org
---

<a name="custom-messages"/>
## [Custom Messages](#custom-messages)
Custom Message give you the ability to write your own message and make it part of a sequence, so that Assistant can use that instead of generating or writing.  
We recommend to let the Assistant write or generate the followup messages at-least, if not the first message. As Assistant will write different message for each lead.

There are some out of the box custom messages (e.g. `post proposal msg`) which you can use but not change. One can edit only those custom messages which are created by him/her. If you want to change something from a message which cannot be edited by you, then clone that message and create your own.

## Personalization 
Custom message and subject can be personalized by using parameters. Available parameters are: 
- Lead First Name
- LeAd Last Name
- Lead Designation
- Lead Phone Number
- Lead Company
- Lead Industry
- Organisation Name
- Organisation Website
- Assistant Name

One e.g. of the Personalization is, using Assistant name in the Subject or message of a Custom Message which is used by across the Org my multiple users. 

## Image in Email
While text emails give a personal human like touch to the emails, at times you may want to include an image in the email sent by the assistant. You can do so.  
While creating or editing the custom message, click on the image icon in the tool bar, select your image and the image will be inserted at the place of your cursor. 

We recommend to keep the image size small (like less than 200 KB). As well, the dimensions of the image to not more than 700X400, so that the image when visible to the lead does not take the whole screen.

**How to put download button in email body? OR How to add buttons in your email?  OR How to add hyperlink to image buttons?**  

Sometimes, you might want to include a call-to-action (CTA) image in your email and link it to a specific URL. This is indeed possible. 
[Please refer this link.]({{ site.baseurl }}/how-to/how-to-add-hyperlink-to-images/)

## Whatsapp Message
To achieve quick followup reply cycle you may want to use whatsapp messages.

To Create a whatsapp Message You can copy the text from Whatsapp template created & Approved in Sinch Dashboard & Click on _Create Whatsapp Message_ Button on Custom Message Page

You can personlize this message such that dyanamic variables used in these templates will be mapped to 7Targets personlized parameters.

For e.g. if you want **{{1}}** to be mapped with Lead First Name then after personalization it would look like this :```{{1->lead.name}}```

You can also attach Videos upto 16 Mb, Images in jpeg format & PDFs.

## SMS Message
To achieve quick followup reply cycle you may want to use SMS messages.

To Create a SMS Message Click on _Create SMS Message_ Button on Custom Message Page

You can personlize this message such that dyanamic variables used in these templates will be mapped to 7Targets personlized parameters.

For e.g. if you want **{{1}}** to be mapped with **Lead First Name** then after personalization it would look like this :```{{1->lead.name}}```


## Questions answered
- I am unable to edit `post proposal msg`. Kindly advice.
- While creating custom message, if there is some content that needs to be picked from company name of the person or lead, can that be done?
- Can I insert or send an image in the message ? 
- Can I add a call to action (CTA) button in the email ?
- How to put download button in email body?
