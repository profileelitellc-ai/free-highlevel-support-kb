**Date Updated:** 2022-07-07T02:39:28.000Z

Note: Now that Workflows are live in all accounts, you can do everything that Triggers and Campaigns do (and more!), all in one builder! [Click to learn more about Workflows](https://help.gohighlevel.com/support/solutions/articles/48001179678-workflow-builder-overview).

Send an email and/or SMS notification to your client(s) and/or yourself when a lead is added to a campaign:

**TABLE OF CONTENTS**

* [How to send internal notifications for workflows](#How-to-send-internal-notifications-for-workflows%3A)
* [Rate limiting on Workflow Notifications](#Rate-limiting-on-Workflow-Notifications)
  
  
# How to send internal notifications for workflows:

  
## Set up a new workflow:
  
  
Click on Start from scratch

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48187640982/original/W7N53A7jRYMkfovt68Zl0xwCszrwqCnfwA.png?1644273935)
  
  
Click on Create workflow
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48187641014/original/Ym9ONXpNJz1suApJvg8ScOvgMnLaDQ3AGA.png?1644273948)
  
  
Click on Add New Workflow Trigger
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48187641031/original/wg8dhPS7alLIU9mtDZK2IiqjrACR883CNw.png?1644273963)  
  
  
Once you configured the workflow trigger:
  
  
Click on Add your first Action

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48187641108/original/InuuOM18OGY_aAIMlGibQLf_YB9IqehKBA.png?1644274015)  
Click on Send Internal Notification
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48187641189/original/KC-4voBjEE-7ueP_CUBYergYsq3TBABUlg.png?1644274083)
  
  
Choose the type of notification:  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48187641355/original/cZ3gsmOHHLQvxqoTAlx_CldWwKwXhpJRzw.png?1644274196)
  
  
Email notification
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48187641351/original/rndkpAofMfCcWWyaCSjPSeHW97FVIQl1kA.png?1644274188)
  
  
Internal notification:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48187641339/original/viF9OCdPD7JRG0C96GaaVSqKrPBSCupE1w.png?1644274180)
  
  
SMS notification
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48187641412/original/BM0tnQY0tkOKGt4tP9ArIMKKzykAO7bHeg.png?1644274226)
  
  
# Rate limiting on Workflow Notifications

  
We have added Rate Limiting for Internal Notification action of workflows.

The current rate limits are

* 500 notifications / 5mins for each user (Per workflow)  
   * In the case of email, its 500 notifications per 5 mins, per user email  
   * In the case of SMS, its 500 notifications per 5 mins, per user's phone  
   * In the case of in-app notifications, its 500/5mins per user Id

We will skip any notifications that are sent after breaching this limit.

Why was this done, and how will this help?

* Because no limit was enforced, there were several updates made to a specific conversation of a user.  
   * Let's say you put 300k contacts into a workflow  
   * And in the internal notification you are sending a mail to a particular user (in most cases we have seen customers set up to send a notification to themselves)  
   * Now this particular user mail, will get 300k emails.  
   * Because of this, the conversation of this user will be updated 300k times, within a few seconds/minutes.  
   * This introduced an overall delay in processing workflow actions.

The rate-limiting should have good gatekeeping for these events, and also prevent customers to send bulk emails to a particular user
  
  