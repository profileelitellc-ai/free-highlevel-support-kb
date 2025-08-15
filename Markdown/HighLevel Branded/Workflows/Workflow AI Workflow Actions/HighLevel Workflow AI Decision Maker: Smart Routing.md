**Date Updated:** 2025-07-23T19:53:08.000Z

This article will show you how to use the **Workflow AI - Decision Maker** to automatically route contacts through different paths based on their engagement, company size, behavior, and more. With just plain English instructions, you can let AI decide the smartest route—no complex logic trees required!

---

**TABLE OF CONTENTS**

* [What is Workflow AI - Decision Maker?](#%E2%80%8B%E2%80%8BWhat-is-Workflow-AI---Decision-Maker?)
* [Key Benefits of Workflow AI - Decision Maker](#Key-Benefits-of-Workflow-AI---Decision-Maker)
* [How To Set Up Workflow AI - Decision Maker](#How-To-Set-Up-Workflow-AI---Decision-Maker)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

---

# **What is Workflow AI - Decision Maker?**

  
**Workflow AI - Decision Maker** acts as an intelligent routing engine inside your workflows. Instead of relying on if/then rules or manual logic, you simply describe the conditions using plain English. The AI evaluates each contact’s data and sends them down the most appropriate branch.

---

# **Key Benefits of Workflow AI - Decision Maker**

  
Workflow AI saves time and improves routing accuracy with minimal setup.

  
* **Reduces Workflow Maintenance:** Once set up, the AI dynamically adapts to changes in contact data, reducing the need to manually update multiple filters and logic rules.
* **Scales Easily with Growth:** Whether you’re routing hundreds or thousands of contacts, the AI handles complexity and volume without slowing down your operations.
* **Eliminates Human Error:** By relying on logic-driven automation, you remove inconsistencies that come from manual decision-making or missed conditional paths.
* **Plain-English instructions:** no coding or rules required.

---

# **How To Set Up Workflow AI - Decision Maker**

  
Learn how to insert the AI action into your workflow and set up dynamic branches based on your criteria.

  
### **Choose or Create a Workflow**

  
Navigate to **Automation** in the left menu. You can either select an existing workflow from the list or click **Create Workflow** to build a new one from scratch, a template, or a recipe.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049278232/original/zBrMzFZg9bL3g4cpGMfDcpT4b13-yaTTNg.png?1751534892)
  
  
### **Add the AI Decision Maker**

  
Click the **+** icon inside your workflow builder where you want to place the action. From the right-side panel, scroll down to **Workflow AI** and select **Workflow AI - Decision Maker**.

  
Make sure to set up a workflow trigger (like “Contact Changed” or “Form Submitted”) before adding any actions, including the AI Decision Maker.
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049278516/original/jtmF7ZPjWmVgvIsYPBEjocD9D6u9MEmPvA.png?1751535045)
  
  
### **Name the Action**

  
Give your action a clear and relevant name under **Action Name**. This helps you easily identify it later in your workflow, especially if you’re using multiple AI or branching steps.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049278621/original/ekJappkUudF3mFUyu3XBJwM3h6V-uPxbMw.png?1751535105)
  
  
### **Write Clear AI Instructions**

  
Use the **Instructions** field to describe what the AI should consider when routing contacts. Be specific about what to evaluate (e.g., engagement score, industry type).

  
Use the **custom value icon** (tag icon) to insert contact fields like {{contact.engagement\_score}} or custom data. This ensures the AI uses actual contact data to make decisions.

  
**Good example:** Look at the contact's engagement score and company size.
 
If the engagement score is over 60 OR they work at a large company, send them to sales. 

If the engagement score is between 30-60 and it's a small/medium company, send them to email nurturing. 

If the engagement score is under 30, send them to a re-engagement campaign.

  
**Important:**

  
To make smart decisions, the AI needs information about your contacts. Use the custom value picker (tag icon) to add contact fields, custom fields, or data from previous workflow steps. Without this context, the AI can't make informed decisions.

  
**Examples of useful information:**

Contact details: {{contact.email}}, {{contact.phone}}

Custom fields: {{contact.lead_score}}, {{contact.company_size}}

Tags: {{contact.tags}}

Previous workflow data: Results from forms, surveys, or other actions
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049278886/original/-f-OAPOMaCtFuuq1ulJxIoqeGxZZvCIeLg.png?1751535240)
  
  
### **Add Business Context**

  
In the **Information** field, provide background data to help the AI make more informed decisions—like support volume, customer segments, or business priorities. The more relevant your context (e.g., audience type, product use case), the more accurate and tailored the AI’s routing logic will be.

  
**Example:** We sell software to companies with 10-500 employees.
 
Small companies have 1-50 people, medium have 51-200, large have 200+.
 
Engagement scores go from 0-100. Our sales team can handle about 20 new leads per week.
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049278989/original/RDi5Z9gicIPnBnQ7IdIXxsmTLKaDWO26mw.png?1751535298)
  
  
### **Default Branch**

  
The **Default Branch** is automatically included and acts as a safety net for contacts who don’t meet any of the other branch conditions.

  
* **Branch Name**: This is locked in as “Default Branch.” It ensures there’s always a path for unmatched contacts.
* **Description**: Explains when the contact will land here — typically if none of your rules apply.
* **Branch Key**: A unique identifier (like none) used internally. It helps track which contacts went down this fallback route.

  
**Note:** You cannot delete or rename the Default Branch. It’s essential for uninterrupted contact flow.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049279785/original/VpVHdVlwn3XfreRU15hw_jWSNNv4jd4EXQ.png?1751535813)
  
  
### **Add a Custom Branch**

  
Create additional branches to route contacts based on unique criteria. In this example, the “Send Discount Offer” branch targets users eligible for a limited-time promo.

  
* **Branch Name**: Clearly label the outcome (e.g., “Send Discount Offer”).
* **Description**: Specify when contacts should enter this path.
* **Branch Key**: Enter a short, unique identifier (e.g., send\_discount\_offer) used for internal tracking and AI routing.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049279653/original/w9ZNYUTkW0lZkuVBVXfD0WQH4gteVzcN0A.png?1751535724)
  
  
### **Add M** **ore Branches**

  
Click **\+ New Branch** to define additional paths for contacts based on unique conditions. Each branch should include a clear name, a short description of when it’s used, and a unique key for tracking. This lets you tailor follow-ups for different audiences—like sending discount offers, product education, or case studies—based on what matters most to each group.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049280003/original/6iGQ64wewpo88MJyRNwWX7Hcqx7YiGexUw.png?1751535950)
  
  
### **Save the Action**

  
Once all your branches are added and configured, click **Save Action** to finalize the AI Decision Maker setup. This locks in your instructions and branch logic, allowing the workflow to begin making smart, automated decisions.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049280124/original/o3ZPJOOtDkYHS-2poYHl7YZp-_8bDL68aA.png?1751536037)

---

# **Frequently Asked Questions**

  
**Q: How does the AI decide where to send someone?**

It reads your instructions and uses the contact’s data (like engagement score, company size) to select the matching branch.

  
**Q: What if someone doesn’t match any rules?**

They automatically go to the Default Branch.

  
**Q: Can I delete or edit the Default Branch?**

No, it’s permanent and ensures fallback routing.

  
**Q: How do I check where a contact went?**

Use the **Execution Logs** tab in your workflow to see the path taken.

  
**Q: Can I use fields from forms or surveys?**

Yes! Include data from previous steps or custom fields using the variable picker.