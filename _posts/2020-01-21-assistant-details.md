---
date: 2020-01-21
title: Assistant Details
video_id: ELaE7f0mi4A
description: Assistant Behavior, Profile and  Defaults
type: Video
sidebar:
  - {id: assistant-profile, text: Assistant Profile}
  - {id: assign-assistant-to-user, text: Assign to User}
  - {id: assistant-manager, text: Assistant Manager}
  - {id: assistant-default, text: Assistant Defaults}
  - {id: multiple-assistants, text: Multiple Assistants}
  - {id: assistant-preference, text: Assistant Preference}
  - {id: auto-activate-new-leads-when-plan-capacity-becomes-available, text: Auto Activate New Leads}
  - {id: lead-name-for-emailcc, text: Lead name for EmailCC}
  - {id: reserve-lead-limit-for-emailcc, text: Reserve lead limit for EmailCC}
  - {id: questions-answered, text: Questions answered}
categories:
  - getting-responses
---

Assistant has the responsibility of communicating with the lead with an intent of getting a meeting. Assistant becomes a virtual team member in your team. 

One important behavior of the assistant is to stop sending more emails on receiving a response from the lead.

Assistant has a default recommended schedule of 7 follow-ups with increasing duration between the follow-ups. User has an option to use custom schedule and change the default schedule too.

Assistant optimizes the email send time for scheduled emails of individual lead, this is done based on when(time) that specific lead opened already sent emails. Each person email checking habits are different, some do in morning, some while lunch and all. Assistant does this hyper-personalization so that the chances of lead reading the email increases. This is `Send Time Optimization`.  

## Assistant Profile
Name, Avatar, Email, Phone Number and Signature represents the Assistant identity. 

Leads see Name, Email, Phone Number and Signature of the Assistant and these can be edited as appropriate. Phone number is also used to notify you of the WARM and HOT leads on WhatsApp. 

At present you cannot add a image/logo to the signature. 

## Assign Assistant to User
Assistant being specific to an industry and offering can be used by multiple users in your organization.  

As an org admin, after a user is invited in 7Targets, you can assign an existing assistant to that user. This user would be able to use the assistant and need not create a new one unless required.  

This helps make sure that the knowledge and expertise of the assistant is maintained and used by multiple users.  

Each user would see his/her own leads only, unless user is an org admin.  

## Assistant Manager
Each assistant typically has just 1 user assigned to her. And that person is like an Assistant Manager for that Assistant, because he can see all the activities of that assistant for all leads the assistant is working on.

Some organisations, assign multiple users to same assistant. In this case, the assistant does not share one users leads with another user. Each user can only see the leads he/she assigned to the assistant.  

At times, there is a need where a given team lead (or a manager) in your company may want to see all the work an assistant is doing even if the manager has to not assigned those leads to the assistant. This is where Assistant Manager concept comes in. 

As an org admin, you can make a user **Assistant Manager** for a particular Assistant.

Once a user is an Assistant Manager for an Assistant, then the user would be able to:

- view and edit the leads of other users for that Assistant
- assign or add leads to that assistant for other users of that Assistant
- change ownership of leads from one user to another of that Assistant

When you need another pair of eyes on your leads, you can make someone from your team an Assistant Manager for a given assistant. That person can help dive deeper into checking the status of all leads that assistant is working on, irrespective of who assigned the leads to that assistant.

## Assistant Default
Assistant has many defaults which are self explanatory. Some of the important ones are mentioned below:

- `Brochure URL` Assistant will embed this URL in the email when responding to requests for Brochure
- `More Context` and `More Information` are the defaults to be used when not provided while adding the leads
- `Shared Calendar URL` If the value for this is provided while Edit Assistant then Assistant will add it in the signature with `Book a Meeting` link. One can create a shared calendar using some service like [Calendly](https://calendly.com/){:target="_blank" rel="noopener"}  
- `Lead at Risk Reminder` Assistant will remind you after every 2 days(can be changed) for 5 times if you forget to reach out to responded leads. Period between each reminder is configurable from `Edit Assistant->Defaults`  
- `Default Schedule` Assistant uses this schedule by default for the added leads. While you can provide the schedule when adding leads from the 7Targets UI. Providing the schedule when adding leads from CRM or by copying Assistant in the email sent by you to your lead is not possible, so in these scenarios the default schedule is used by the assistant. Value of default schedule can be changed by going to Assistant->Edit Assistant.
- `Default EmailCC Schedule` is used by the assistant when assistant is copied in the email by the user with the lead. For EmailCC schedule, Assistant will start the with second message in the sequence. Your email where you Cc'ed/Copied the assistant is considered as the first email. More details about how the name of the lead works is here [Lead name for Email CC](#lead-name-for-emailcc)

## Multiple Assistants
You can create multiple assistants for yourself. Assistants cannot be shared or assigned to other users in the Org. 

We recommend to have `geography and vertical specific` assistants. So that the assistant is trained for nurturing the leads of that vertical with specific nurturing material.

## Assistant Preference
There are various Preferences you can set for the assistant and are self explanatory on the Assistant Preference page. Some of the preferences are explained below:  

## Auto Activate New leads when plan capacity becomes available
If this preference is on (Which is the default) then Assistant will automatically activate the leads with New status, if the capacity becomes available as per the Plan. 

Assistant checks for any New leads every day at 10:00 AM GMT and if there is capacity available then these New leads are activated, i.e. restarted, so that emails starts going to these leads as per the schedule. 
To know what is New lead or lead with state New, refer [Lead States](../../assigning-leads/lead-responses/#lead-state)

## Lead name for EmailCC
Assistant tries to pick the name from the lead email if available. For e.g. if the lead email is with name like `Sanju Burkule <sanju.burkule@7targets.com>` then Assistant will extract the first_name and last_name correctly. While typing the email in your email client you can provide the name and email id like above. 

But, in case the name is not available in the email, i.e. in the email only the lead email is present (`sanju.burkule@7targets.com`) then Assistant cannot know the name. And will default to the value in the preference  
__Default lead name to use when assistant is Cc'ed and lead name not given__.  
Default value for this is `Sir/Madam` and you can edit to provide any other value as default. 

But, if you save the preference with no value in it. Then Assistant will use the string in front of the `@` in the lead email as name. For e.g. if the lead email is `sales@somecompany.com` then the first name will be taken as `Sales`. To avoid situation where the email goes as `Hello Sales` it is recommended to set some default and not let this situation come. 

## Reserve lead limit for EmailCC
By default 5% leads are reserved for EmailCC source, so that when users copies the assistant in an email sent to lead, it has the lead limit availability to process. You can change this value from the Assistant preference.  

Assistant will not allow other leads sources, like bulk file upload, to use this reserve. 

## Questions answered
- Can I add logo in the signature ?
- Can we integrate with shared calendar service like Calendly ? 
- Will assistant stop sending emails after response is received ? 
- What will assistant do when it received an email response ? 
- Can I have multiple Assistants ? 
- Why and when should I use multiple assistants ? 
- Should I invite user to 7Targets or create an assistant for that user. Cannot assign assistant from one user to other ?
- What is send time optimization ?
- Can I share my assistant with other users of my org ? 
- Can other users in my org use the same assistant ? 

