**Date Updated:** 2025-07-28T23:51:00.000Z

Easily automate actions when a coupon code is applied at checkout. This article walks you through everything you need to know, from setup to key benefits, so you can seamlessly trigger workflows whenever a customer applies a coupon code, regardless of whether they complete the purchase. Perfect for reward follow-ups, internal alerts, and sales optimization.

---

**TABLE OF CONTENTS**

* [What is the Coupon Code Applied Workflow Trigger](#What-is-the-Coupon-Code-Applied-Workflow-Trigger)
* [Key Benefits of Coupon Code Applied Workflow Trigger](#Key-Benefits-of-Coupon-Code-Applied-Workflow-Trigger)
* [Configuring Coupon Code Applied Workflow Trigger](#Configuring-Coupon-Code-Applied-Workflow-Trigger)
* [Available Filters](#Available-Filters)
* [Recommended Workflow Actions for Coupon Code Usage](#Recommended-Workflow-Actions-for-Coupon-Code-Usage)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)

---

# **What is the Coupon Code Applied Workflow Trigger**

  
The Coupon Code Applied trigger is used to initiate a workflow the moment a coupon code is applied to an order during checkout. The workflow fires regardless of whether the order is completed, allowing businesses to automate follow-ups, tagging, internal notifications, or targeted sales offers in real-time when discount codes are used.

It’s an essential tool for sales teams and marketers who want to monitor coupon code usage and act immediately, without waiting for an order to finish processing.

---

## **Key Benefits of Coupon Code Applied Workflow Trigger**

  
* **React Instantly to Coupon Code Usage:** Trigger automations as soon as a coupon is applied at checkout
* **Abandoned‑Cart Recovery:** Remind shoppers who applied a coupon but failed to finish checkout, nudging them to return and complete their purchase
* **Personalized Upsells:** Detect the coupon type or value and present tailored upsell offers that feel relevant and helpful
* **Accurate Targeting with Advanced Filters:** Fire actions based on coupon code, type, order value, product, and more
* **Operational Efficiency:** Notify teams or tag contacts when specific discount codes are applied to monitor performance

---

## **Configuring Coupon Code Applied Workflow Trigger**

  
To set up this trigger, head to your workflow builder and follow these steps:
  
  
#### **Step 1:**Add the Trigger to Your Workflow

  
* Navigate to **Automation > Workflows**
* Either create a new workflow or edit an existing one
* In the workflow builder, click **\+ Add New Trigger** to get started

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050382194/original/F9qxCGgkR-XZ5jtwTc9S9hWkflT9XX_HwQ.png?1753365840)
  
  
#### **Step 2:** Choose the Trigger Type

  
From the list of available triggers, scroll to the **Payments** section and select **Coupon Code Applied**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050382304/original/QA74NLhgPeH9Qd5PPf8TA7dXIl5KJ_XHcg.png?1753365909)
  
  
#### **Step 3:** Name Your Trigger

  
* Provide a descriptive name in the **Workflow Trigger Name** field to keep your workflow organized.
* Example: _"15% off Coupon Code Applied on Product 1"_

  
`![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050382386/original/-YcR2-lw0tkrVI_cuCbmWTxdhzATBG4GfA.png?1753365945)`
  
  
#### **Step 4:** Apply Filters to Target Specific Scenarios

  
* After naming the trigger, you can apply filters to narrow down exactly when this workflow should fire
* To add filters, click **\+ Add Filters**
* Each filter comes with specific operators (like _Is_, _Contains_, _Greater Than_, _Before/After_) to precisely target the conditions you care about. [Click Here to See List of Available Filters](#Available-Filters)

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155050382758/original/fAA2RXLA9XQtmfmX7dzdf1Oo2QvMndMwww.png?1753366194)
  
  
#### **Step 5:** Save and Build the Workflow

  
* Once your trigger and filters are configured, click **Save Trigger** and start adding your desired actions to the workflow.
* When finished, use **Test Workflow** to confirm everything’s working as expected, then **Publish** the workflow to activate it.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049297661/original/PtVRE6cOM4E2TbgTZG2g_JvxWNFrchlcZw.png?1751548691)

---

## **Available Filters**
  
  
| Filter                        | Operator(s)                                                                                                                         | Input Type                                                     |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| Coupon Code                   | Is Any Of / Is Empty / Is None Of / Is Not Empty                                                                                    | Multi-Select Dropdown of Coupon Codes                          |
| Coupon Name                   | Is Any Of / Is Empty / Is None Of / Is Not Empty                                                                                    | Multi-Select Dropdown of Coupon Names                          |
| Coupon Type                   | Is / Is Empty / Is Not / Is Not Empty                                                                                               | Amount / Percentage                                            |
| Coupon Value                  | Equals To / Greater Than / Greater Than or Equal To / Is Empty / Is Not Empty / Is Not Equal To / Less Than / Less Than or Equal To | Numerical Input Box                                            |
| Order Value (Before Discount) | Equals To / Greater Than / Greater Than or Equal To / Is Empty / Is Not Empty / Is Not Equal To / Less Than / Less Than or Equal To | Numerical Input Box                                            |
| Product Collection            | Contain Any / Is Empty / Is None Of / Is Not Empty                                                                                  | Multi-Select Dropdown of Product Collections                   |
| Product Type                  | Contain Any / Is Empty / Is None Of / Is Not Empty                                                                                  | Multi-Select Dropdown of Product Types (One Time vs Recurring) |
| Product(s) In Order           | Contain Any / Is Empty / Is None Of / Is Not Empty                                                                                  | Multi-Select Dropdown of Products                              |
| Source                        | Is / Is Empty / Is Not / Is Not Empty                                                                                               | Single-Select Dropdown                                         |

---

## **Recommended Workflow Actions for Coupon Code Usage**

  
Once your **Coupon Code Applied** trigger is set up, consider adding these actions to optimize your sales and customer experience:

  
* **Send Email:** Notify the customer with a personalized message acknowledging their coupon code use
* **Assign to User:** Automatically assign the contact to a sales or support user for follow-up
* **Add Tag:** Apply tags to the contact based on the coupon code they applied
* **Internal Notification:** Alert your team when high-value or special coupons are used
* **Create/Update Opportunity:** Route the lead into your sales pipeline if applicable

---

## **Frequently Asked Questions**

  
**Q: Will the trigger work if the customer doesn’t complete the checkout**  
Yes, this trigger fires the moment a coupon is applied, regardless of whether the customer completes the order.

**Q: Can I track which products the coupon was applied to?**

Yes, use the Product(s) in Order and Product Collection filters to narrow down based on product selections at the time the coupon was applied.

  
**Q: What happens if I don’t add any filters?**

If no filters are applied, the workflow will trigger for any coupon code applied at checkout. It’s best practice to use filters like Coupon Code Is or Coupon Type Is to target specific campaigns.

**Q: Can I trigger actions based on order value before and after discounts?**

Yes, you can use Order Value (Before Discount) and Order Value (After Discount) filters with operators like Greater Than and Less Than to control when the workflow fires.

  
**Q:Are scheduled orders supported with this trigger?**  
No, this trigger only fires when a coupon is actively applied at checkout.

---

## **Related Articles**

  
* [Workflow Trigger – Coupon Code Redeemed](https://help.gohighlevel.com/en/support/solutions/articles/155000005658)
* [Workflow Trigger – Coupon Redemption Limit Reached](https://help.gohighlevel.com/en/support/solutions/articles/155000005660)
* [Workflow Trigger – Coupon Code Expired](https://help.gohighlevel.com/en/support/solutions/articles/155000005661)
* [How to Create Coupons for Products](https://help.gohighlevel.com/en/support/solutions/articles/48001224172)
* [Coupon Application on Subscription Products](https://help.gohighlevel.com/en/support/solutions/articles/155000004886)