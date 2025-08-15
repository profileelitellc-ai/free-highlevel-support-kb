**Date Updated:** 2024-10-25T19:21:28.000Z

Voicemails are a great way to reach customers and let them know about your business. Voicemail drops are a quick and inexpensive way to determine if your messages are getting through. Your voicemail drop could be the first step towards increasing sales and customer satisfaction. Get started right away by ordering your free voicemail drop from our website.

  
In this article, we will cover Call and Voicemail drop events.

---

#### **Covered in this article:**

#### [**How to set up automated calls and voicemail drops in Workflows**](#How-to-set-up-automated-calls-and-voicemail-drops-in%C2%A0Workflow)

* #### [After you configure the workflow trigger](#After-you-configure-the-workflow-trigger)
* #### [By default, the call whisper states, "You have a new lead, John Smith. Press any button to connect".](#By-default,-the-call-whisper-states,-)

#### [**How to set up automated calls and voicemail drops in Campaigns**](#How-to-set-up-automated-calls-and-voicemail-drops-in-campaigns)

####   
[**FAQ's**](#FAQ's)

* #### [My voicemail file is not working](#My-voicemail-file-is-not-working).
* #### [Are Voicemail drops legal?](#Are-Voicemail-drops-legal?)
* #### [A quick video on how they work and some gotchas to be aware of.](#A-quick-video-on-how-they-work-and-some-gotchas-to-be-aware-of.)

---

## **Prerequisites:**

\- You have already purchased a number in your subaccount ([LC Phone Guide](https://help.gohighlevel.com/support/solutions/articles/48001223546-what-is-lc-phone-system-)) or ([Twilio Guide](https://help.gohighlevel.com/en/support/solutions/articles/48000981420))

\- You have pre-recorded Audio files that are **mp3/wav files** (**64kbps** ) as [outlined here](https://help.gohighlevel.com/support/solutions/articles/48000981433-voicemail-drop-file-conversion)

\- You have taken the user's consent for automated calls in order to drop Voicemails.

---

# **How to Set up Automated Calls and Voicemail Drops in** **Workflow**

  
Once you are in the sub-account, click "**Automation"** from the left side navigation menu.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035413156/original/k7jXvtYZTRESWHqEYOR5D7I0nH0kdZEsLA.png?1729857742)

  
Click on "+ **Create Workflow**."

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035413228/original/7pQt9biMkNvBRJF_PPIz6oNeEEl1cB_wnw.png?1729857765)

  
Click on " + **Start from scratch."**

**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035413281/original/Jz40ejD47ekj6Js_oYER7fxCZnWVZ9YDvw.png?1729857796)**

  
Select a workflow trigger for your call /voicemail drop action. In this example, we have used "Contact Changed" trigger.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035402405/original/C6XyM-AJgY72eq09KMnNYkyH-VK8vHS7gA.png?1729850513)

  
To add the workflow action, click **"+"** button 

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035402488/original/UqreaGPzLJAjduU1cTmHji7LDIUdvq5NZA.jpeg?1729850573)

  
You can either scroll down or search for "Assign to User" action. Click on "**Assign to User."**

#### **![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035413050/original/BZdwLy-70MR1Zvd3OcjytwhUvjdAAl1nKQ.jpeg?1729857672)**

#### **Users** 

Select user from the drop down menu If you want the calls to go to a dedicated team member (See [assigned user's phone number configured](https://gohighlevelassist.freshdesk.com/support/solutions/articles/48001152124-phone-numbers-for-users-assign-twilio-numbers-to-users).)

If no one is assigned, the calls will go to the phone number you have saved in your business profile as a company phone number. (see [Inbound Call Routing - Explained](https://help.gohighlevel.com/en/support/solutions/articles/48000981432).)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035412395/original/Ig0TBuIY_tjSdhuHE86IoskvVe79OVHgKA.png?1729857232)

  
**Only Apply To Unassigned Contacts**

In the previous step, we choose the team member who will be automatically assigned all the new contacts that enters into this workflow.  
  
Now this toggle option gives you the ability to decide weather you want to assign the newly added contacts to the same user even if the contact is already assigned to any of the team member before it entered into this workflow or you want to stop assigning such contacts.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035412408/original/nTIj7RFjfgzxx6YVCukrs5ZQEhNLqeUNhQ.png?1729857249)
  
  
**Save Action**

Don't forget to **Save action** before you go back to the workflow builder page.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035412461/original/Q-3WZFFKggFOmJTBYAsxERr9Tj_3avlrTA.png?1729857269)

  
Lets Add "Call" action. Just click the **"+"** button and select **"Call"** action.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035402757/original/TB35W_xM1A0pZgdqnM1xlqF85cCOAhaCIw.jpeg?1729850714)

  
**Call Whisper**

You can modify the Call whisper message here:  
By default, the call whisper states, **"You have a new lead, John Smith. Press any button to connect"**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035413386/original/DIUhE5q_TeBTuFr2LGpjI44ntHWwgDlFfw.jpeg?1729857878)

  
**Voicemail Detection**

When the lead can't answer the call, you will hear this message: "Couldn't connect with the lead," and the call ends. You can't leave a personalized voicemail if this occurs.  
  
To leave a personalized voicemail with our Call event, go to the settings of the call step, and you can turn on "**Disable Voicemail Detection."**  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035404475/original/kSHRdZjE2ZaBTbIXkodArtZ9eceQf5Qwow.png?1729851810)

  
**Connect Call After Keypress**

Use this toggle if you want to connect the call only after a user press any key.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035408749/original/UzHDqdtrnn38ng7A_4rgotvAYT3oV6fzrQ.png?1729854503)  

**Voicemail Action**

Now lets see how to add "Voicemail" action. for that, you will be using the same "+" button to add a new workflow action. Once you see the page with all the workflow actions, scroll down to find "Voicemail" option and click on it to proceed ahead.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035413480/original/nRmBvmYdsi2WX9nOo8DkglqksFCKQYkFTA.jpeg?1729857925)

  
**Upload File**

You can upload the recorded voice using the upload file here. Be sure to click **"Save Action"** once you have successfully uploaded the file.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155035413516/original/hWIhRMNZ7-eihgYlBhYVmP_Yju2XwsOzMQ.jpeg?1729857951)

---

# **FAQ's**

### **My voicemail file is not working.**

1\. go to <https://online-audio-converter.com/> and upload the voicemail file. Otherwise, you can create a new file here <https://www.rev.com/onlinevoicerecorder>

  
2\. Select **64kbps MP3**, the lower the better

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48189712460/original/ZTtqkvqzGQ7rQJIEhac3liq96BLgoytlNQ.png?1644711271)

  
3\. Upload back to HighLevel voicemail campaign/workflow

  
### **Are voicemail drops legal?**

Voicemail drops are legal as long as you have the user's consent before dropping the voicemail. Else they are illegal. The TCPA applies to ringless voicemail drops because they are considered a form of communication that uses an automated dialing system and a prerecorded message. Therefore, you need to have prior express consent from the recipients before sending them ringless voicemail drops. Otherwise, you may face lawsuits and fines from the Federal Communications Commission (FCC) or private parties.

  
### **Why am I not able to drop more Voicemails?**

Voicemail drop limits ramp up as you spend more time with us.

Day 1: 100 drops per day

Day 2: 200 drops per day

Day 3: 300 drops per day ...

Day 7: 700 drops per day

Day 7 onwards: 2000 drops per day

  
If you would like to increase these limits, please reach out to our support team.

  
### **A quick video on how they work and some gotchas to be aware of:**

  
###   

**TLDR; Voicemail drops rely on a carrier trick, this is how all voicemail drops work, and as a result they only work about 70% of the time.**
  
  