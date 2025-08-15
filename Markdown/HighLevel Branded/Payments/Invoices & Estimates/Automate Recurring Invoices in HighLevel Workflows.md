**Date Updated:** 2025-06-28T02:33:57.000Z

Easily automate your recurring billing cycles in HighLevel by using the Send Recurring Invoice action in a workflow. Whether you manage memberships, agency retainers, or SaaS subscriptions, this native automation eliminates manual invoicing, keeps payments on schedule, and reduces the need for third‑party tools.

---

**TABLE OF CONTENTS**

* [What is Recurring Invoices in Workflows?](#What-is-Recurring-Invoices-in-Workflows?)
* [Key Benefits of Recurring Invoices in Workflows](#Key-Benefits-of-Recurring-Invoices-in-Workflows)
* [Prerequisites](#Prerequisites)
* [Recurring Invoice Configuration Settings](#Recurring-Invoice-Configuration-Settings)
* [How to Set Up Recurring Invoices in Workflows](#How-to-Set-Up-Recurring-Invoices-in-Workflows)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)[](#Related-Articles)

---

# **What is Recurring Invoices in Workflows?**

  
Recurring Invoices in Workflows automates scheduled billing inside your workflows, allowing invoices to send automatically while you focus on customers. In the visual Workflow Builder you can set start dates, stop rules, frequencies, and Auto‑Pay—keeping cash flow predictable without manual effort. 

---

## **Key Benefits of Recurring Invoices in Workflows**

  
Set up recurring invoices in just a few clicks and enjoy hands‑free billing, flexible schedules, and built‑in auto‑pay—all without 3rd party tools.

  
* **Time Savings:** save time by cutting out manual invoice creation and follow‑up
* **Flexible Cadence:** daily, weekly, monthly, or yearly schedules to fit any plan
* **Start‑Date Control:** begin at the contact’s trigger date or a fixed calendar date
* **Stop Rules:** choose never‑ending or end after X occurrences
* **Auto‑Pay:** charge a stored card automatically after the first successful payment
* **Error Reduction:** eliminates missed or duplicate invoices
* **Workflow Integration:** billing events stay in sync with tags, emails, and follow‑ups

---

## **Prerequisites**

  
Having the essentials in place ensures your recurring invoices run without a hitch.  
  
* **Invoice Template:** Create at least one template in **Payments → Invoices**
* **Payment Gateway:** Connect Stripe (or another supported gateway) in **Payments → Integrations**

---

## **Recurring Invoice Configuration Settings**

  
The Send Recurring Invoice action is highly customizable. This section breaks down each option so you can tailor billing to fit any plan before you click Publish.
  
  
#### **Start Date Options**

  
The **Start Date** dropdown lets you choose when the schedule begins, ensuring invoices reach customers at the right moment.

  
* Action Date: begins the schedule as soon as the contact hits the workflow trigger (e.g., tag added or contact changed)
* Fixed Date: aligns billing with a specific calendar day (e.g., 1 July, 2025)
  
  
#### **End Criteria and Stop Rules**

  
The **Stop** dropdown controls when the schedule ends, preventing over‑billing or unintended charges.

  
* Never: continues until manually stopped
* After X Occurrences: perfect for installment plans (e.g., 12 monthly payments).
  
  
#### **Recurrence Frequencies**

  
The **Frequency** dropdown determines how often invoices repeat and displays extra selectors (e.g., weekday, month) based on your choice.

  
* Daily: every _N_ days—ideal for high‑frequency payments
* Weekly: send on a specific weekday or on the action date—great for weekly coaching
* Monthly: by date or by week (e.g., 2nd Wednesday)—common for memberships and retainers
* Yearly: choose month and day, every _N_ years—ideal for annual renewals
  
  
#### **Auto‑Pay**

  
Toggle **Enable Auto‑Payment** to charge it automatically after the first successful payment, streamlining collection.  
  
* Gateway Requirement: currently supported with Stripe‑connected sub‑accounts
* First Invoice Must Succeed: card details are stored only after a successful manual payment

---

## **How to Set Up Recurring Invoices in Workflows**

  
Properly configuring the Send Recurring Invoice action takes only a few clicks. Follow the numbered steps below to automate billing without errors.  
  
#### **Step 1:** Navigate to Workflow Builder

  
* From your HighLevel dashboard, navigate to **Automation → Workflows**
* Click the blue **\+ Create Workflow** button in the top‑right corner to create a new workflow

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049011373/original/yFXCqMLZ1da5zLCe_gmAJVo9tSo_FkKRlA.png?1751055820)
  
  
#### **Step 2:** Add Your Workflow Trigger

  
* Within the Workflow Builder, click **\+ Add Trigger**.
* Choose a trigger then click **Save Trigger**.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049011420/original/SNjzL49ekAWIwxNzEbvuYxTHkNSAG8NXYA.png?1751055952)  
  
#### **Step 3:** Insert the **Send Recurring Invoice** Action  
  
* Click the **➕** directly beneath the trigger to add an action
* In the Action search bar, type **Send Recurring Invoice** and select it

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049011469/original/t6Imurq_oLV6Wcv2589mdSQqiAx9dkGi6Q.png?1751056024)  
  
#### **Step 4:** Configure Action Settings  
  
* Name the action so it’s easy to identify (e.g., “Monthly Retainer – Silver”)
* Select **From User** to choose the sender
* Pick an **Invoice Template**
* Toggle **Mode** to Test for trial runs or Live for real billing
* Under **Start Date**, choose Action Date or Fixed Date
* Under **Stop**, select Never or After X Occurrences
* Open the **Frequency** dropdown to pick Daily, Weekly, Monthly, or Yearly and adjust the interval options that appear
* Enter **Days in Advance** to send the invoice _N_ days before the due date
* Toggle **Enable Auto‑Payment** on to store the customer’s card after the first payment and charge subsequent invoices automatically

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049011721/original/RGEE_snKsuGkThmwOpDN7pP090MM6f9uAA.png?1751056997)  
  
#### **Step 5:** Test and Publish  
  
* Once the workflow has been setup, click the blue **Save** button in upper right corner
* At the top of the workflow, click **Test Workflow** to test the workflow
* When everything looks correct, toggle to **Publish** to activate the workflow

  
**Tip:** For a deeper dive into workflow navigation, see [Workflow Builder Walkthrough](https://help.gohighlevel.com/en/support/solutions/articles/155000001254)

---

## **Frequently Asked Questions**

  
**Q: Do I need a payment gateway to send recurring invoices?**  
Yes. Connect Stripe (or another supported gateway) before activating Auto‑Pay or sending invoices.  
  
**Q: What happens if a customer’s card fails during Auto‑Pay?**  
The invoice remains unpaid. Set up a workflow with a Payment Failed trigger to retry and notify the customer.

**Q: Will recurring invoices appear in the customer’s invoice history?**  
Yes—all generated invoices are logged under the contact’s record.

  
**Q: Does the Live/Test toggle affect existing schedules?**  
No. It only controls invoices created after the toggle change.  
  
**Q: Can I send different templates based on contact attributes?**  
Use conditional branches to add multiple Send Recurring Invoice actions with different templates.

---

## **Related Articles**

  
* [How to Create and Use Invoice Templates in HighLevel](https://help.gohighlevel.com/en/support/solutions/articles/155000001297)
* [Stripe Integration with HighLevel](https://help.gohighlevel.com/en/support/solutions/articles/155000005073)
* [Workflow Builder Walkthrough](https://help.gohighlevel.com/en/support/solutions/articles/155000001254)
* [Triggers - Overview](https://help.gohighlevel.com/en/support/solutions/articles/48000982202)