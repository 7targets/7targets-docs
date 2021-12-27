---
date: 2021-12-26
title: How and why assistant check for name email mismatch
#video_id: JC2yJnBXzLM
description: Assistant validates name and email to help you avoid mistakes
type: How-to
sidebar:
  - {id: step-1, text: Upload}
  - {id: step-2, text: Name Email Mismatch email notification}
  - {id: step-3, text: Proceed as is}

categories:
  - How-To
# set: getting-started
# set_order: 3
---

We have seen this happens with some of our customers. By mistake, while working with the excel file to be uploaded, the name and email column values ended up not matching. In one case, it was just one row moved out. i.e. name of the lead was matching with the email in the next row.  

Such mistakes are very costly. In physical world, one would expect the Sales Assistant to identify and let know such inadvertent mistakes. 

7Targets AI Sales Assistant now has this capability. Using machine learning along with a proprietary algorithm, your Assistant will try to identify such mistakes and inform you over email. You can then correct the data and upload the excel file again or "Proceed as is" if required. 

## Step-1 

Upload an excel file. 
[Details on how to add multiple leads](../how-to-add-multiple-leads/)

## Step-2
If Assistant finds that there are more than 50% name email mismatches in your uploaded data then below like email will be received. 

![image](../../images/name-email-mismatch-notification.jpg)

## Step-3
Clicking on the link will open the upload history page.  

If the data is indeed mismatched then you would Cancel this upload, correct the data and upload the excel file again. 

If you think that the data is correct, then you can "Proceed as is".  

![image](../../images/cancel-or-proceed-as-is.jpg)

If you have any further doubts, you can directly mail us at info@7targets.com.