**Date Updated:** 2024-08-01T03:23:48.000Z
  
  
Introducing the quick opt-in option in email unsubscribe workflow.

Problem Statement:

Previously, the process to re-opt into our mailing list after unsubscribing was complicated and lacked a same-window solution.

What We Did:

To address this, we've introduced a quick resubscribe link directly within the unsubscribe success message. Now, if a user unsubscribes by mistake, they can easily opt back in by clicking the resubscribe link. This action will immediately remove the email from the Do Not Disturb (DND) list.

How to Test?

1. Go to Email Marketing.
2. Create and send a campaign to a dummy contact.
3. Click the unsubscribe link in the email.
4. Use the resubscribe link in the success message.

![image](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155030260053/original/sD-Tg6M4xtbOIiUgWMLZb-bIl8IUGtITaQ.png?1722462766)

![image](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155030260055/original/QgHYKCSUHXRJA82Q8TLoBNcrBnpCwx-LdQ.png?1722462766)

1. Check the DND section in contacts.

![image](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155030260054/original/cKJsaMabRC45n3wBpTIWB2__JglwJmk-fA.png?1722462766)

Note:

Users re-opting in may still appear under unsubscribed in campaign statistics. We are working to fix this.