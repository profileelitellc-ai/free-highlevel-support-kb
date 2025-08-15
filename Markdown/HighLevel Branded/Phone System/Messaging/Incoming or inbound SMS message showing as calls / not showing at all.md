**Date Updated:** 2023-02-25T00:38:42.000Z

  
[Try to reset Twilio number if you are NOT on Leadconnector phone system:](https://help.gohighlevel.com/support/solutions/articles/48000981428-deleting-resetting-a-twilio-number)

If resetting the Twilio number is not working, When inbound SMS is not coming into HighLevel:

  
1\. Login to <https://www.twilio.com/login> [](https://www.twilio.com/login)  
  
2\. Go to the top right -> Click **Account** \-> Click **Sub** **accounts**  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48182954716/original/xU1ASMn2bOtT6Y1BdbfgUAYu3F-UlqKoNQ.jpeg?1643126214)

If there are too many subaccounts inside Twilio, you can go back to the agency view in the platform and copy the Account SIN for that location to search in Twilio:

  
If you are on LC phone, please [contact support](https://help.gohighlevel.com/en/support/solutions/articles/48001204857) [](https://help.gohighlevel.com/en/support/solutions/articles/48001204857)

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48282353466/original/1_Ux25zIZeWokpmKPOdKcNy-SXEUJWA6ww.png?1676661550)  
  
  
Now go back to Twilio with the copied Account SID

Search based on the Twilio Subaccount SID in HighLevel agency settings -> Twilio  
Paste the Account SID here and click on it:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48182954706/original/TaZM1HBRp-VAFwRC5VUjjoQfYNndbVXXeQ.png?1643126214)

  
Check if the Twilio number is MMS capable:
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48182954714/original/upUE1TjZVCDpol7AORlv2jGlHDK5qCPJRg.jpeg?1643126214)

  
Click on **Phone numbers:**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48282353637/original/UuPrOZYjpEbL77yl8Mf1o-wEwddnsT-x9g.png?1676661628)  
  
  
Check if it is configured as:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48282353849/original/XX7YyfGy4J3Gb7PbKgDidBzLeG-9eTNk-w.png?1676661731)
  
  
If not, please click the phone number and scroll down to replace the webhook:

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48282354439/original/iA5YWoSchQg-kWVV-CsozA6jMeZYgZs0AA.png?1676662051)
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48282354731/original/3BVPjA6QB80uQ3HQPS6KdPAP3R4GdgavAQ.png?1676662244)
  
  
Click save and

Now you can test again to see if incoming SMS will show up in HighLevel.

  
If you have some messaging service that's connected to the Twilio number, click into the messaging service here:

Note for LC phone that might be the case once signing up for a2p messaging service, don't follow the steps here.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48242937212/original/XUJloEgs-eytrgs7t_X9x16ZzM8_-VLoWA.png?1659550327)
  
  
Click **Sender Pool** on the left

Remove all the Twilio numbers here
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48242937517/original/-jHT_RUA3LzVOOFShxOjAoe_xyqL9J5Dxg.png?1659550417)
  
  
If NOT:

  
Verify if the Twilio number has an icon † next to it

†Can send/receive SMS to domestic numbers only
  
  
Left panel, Click **Monitor** \-> **Messaging**  
  
Put the lead's phone number (remove all phone format) in the TO field:  
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48182954710/original/f5X5OOuNDeeTc2Agj0HwxMhwvB977Efv2g.jpeg?1643126214)  
  
  
Click the Date on the left for further details:  
  
If it says delivered but the contact is not receiving it, grab this Message SID and open a ticket with Twilio support  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48282354195/original/_WhibpjafHDYtBwvExSC0OWlOPUpEv4CEg.png?1676661895)
  
  
If you hover over the records, it will preview the content of the message. What does the status say?
  
  
##   