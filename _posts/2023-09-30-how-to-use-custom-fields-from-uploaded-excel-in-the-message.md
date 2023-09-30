---
date: 2023-09-30
title: How to use custom fields from uploaded excel in the message ?
description: Need to use custom fields or parameters for each lead in the uploaded excel as a personalize parameter or variable in the custom message used in the squence
#video_id: TcibhmCn9gM
type: How-to

sidebar:
  - {id: create-message-with-parameters text: Create message with parameters}
  - {id: upload-excel-with-columns, text: Upload Excel with columns}
  - {id: actual-email, text: Actual Email}
categories:
  - How-To
# set: getting-started
# set_order: 3
---

You'll want to use specific fields unique to each lead from the uploaded Excel sheet, as personalize parameters within the custom messages used in your sequence.

This will help you make your custom messages generic enough.  
e.g. such parameters could be Phone, Project, Investment, Business Problem, Icebreaker, etc.  
You can pass value for these parameters or fields from the uploaded excel. While sending the actual message the value for the excel will be used to replace the Personalize variable/parameter name in the message. 

## Create message with parameters
Simply click on `Personalize` while creating or editing the message. If you want to use a custom field which will come later from the uploaded excel. Type the parameter name (column name of the custom field from excel). Make sure to put the default value.  

Note below conditions, it is for each lead from the excel :  
- **IF** default value is provided and the parameter is uploaded via the excel; **THEN** the value from the excel will be used. Even if the value from excel is `empty`
- **IF** default value is provided and the parameter is not uploaded via the excel; **THEN** the default value will be used
- **IF** no default value is provided and the parameter is uploaded via the excel; **THEN** the value from the excel will be used. Even if the value from excel is `empty`
- **IF** no default value is provided and the parameter is not uploaded via the excel; **THEN** the value for the parameter while sending the actual email will be `empty`

![Personalize Custom Parameters](../../images/personalize-custom-parameters.png)

## Upload Excel with columns
Below is the screen show depicting the excel which is uploading the leads with the custom parameters used while creating the message. Note the value is different for each lead in the excel.

![Excel with Custom Fields](../../images/excel-with-custom-fields.png)

## Actual Email
Now when the actual emails goes out you could see that the actual value was used from the excel. 
Note the screen shot of the email sent as well as scheduled. Schedule email will use the value of the parameter and show the message. 

![Sent Email from timeline](../../images/sent-email-from-timeline.png)
![Scheduled Email from timeline](../../images/scheduled-email-from-timeline.png)