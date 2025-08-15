**Date Updated:** 2025-07-23T23:36:35.000Z
  
  
This guide walks you through the new SaaS Sub-Account Cancellation Flow customization options, available to agencies using the SaaS Configurator. It explains how you can personalize the cancellation experience for your clients, offer discounts to reduce churn, track cancellation activity, and redirect users if needed. If you're looking to gain better control over subscriber cancellations and improve retention, this documentation is for you.

---

**TABLE OF CONTENTS**

* [What is the Custom SaaS Cancellation Flow?](#What-is-the-Custom-SaaS-Cancellation-Flow?)
* [Key Benefits of the Custom Cancellation Flow](#Key-Benefits-of-the-Custom-Cancellation-Flow)
* [Global Toggle — Allow Clients to Cancel Subscription](#Global-Toggle-%E2%80%94-Allow-Clients-to-Cancel-Subscription)
* [Manage Cancellation Reasons](#Manage-Cancellation-Reasons)
* [Offer Discount to Retain Clients](#Offer-Discount-to-Retain-Clients)
* [Redirect Users to an External Page](#Redirect-Users-to-an-External-Page)
* [Track Cancellation Activity with Activity Logs](#Track-Cancellation-Activity-with-Activity-Logs)
* [Preview the Cancellation Flow](#Preview-the-Cancellation-Flow)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)

---

# **What is the Custom SaaS Cancellation Flow?**

  
Custom Cancellation Flow replaces the default “one-click cancel” with a branded, multi-step journey. At each stage—reason collection, discount offer, external redirect—you decide the wording, incentives, and next actions, ensuring clients encounter an intentional retention experience instead of an abrupt exit.

---

## **Key Benefits of the Custom Cancellation Flow**

  
* **Capture Exit Insights**: Gather structured and open-ended cancellation reasons to inform product, pricing, and onboarding improvements.
* **Reduce Churn**: Present time-bound percentage discounts during the exit flow to persuade wavering clients to remain subscribed.
* **Drive High-Touch Saves**: Redirect cancel-clickers to external concierge pages, surveys, or booking links for personalized retention efforts.
* **Maintain Full Visibility**: Track every cancellation attempt or deflection in real-time Activity Logs for transparent reporting and coaching.
* **Iterate Without Code**: Update reasons, offers, and copy on demand, enabling rapid A/B testing of retention tactics, without the need for coding

---

## **Global Toggle — Allow Clients to Cancel Subscription**

  
Turning this master switch **ON** reveals the “Modify / Cancel” button inside every sub‑account’s Billing Dashboard. Turning it **OFF** hides all cancellation options, deferring control entirely to the agency.  
  
* Location: **Agency View** **→ SaaS Configurator → Cancellation Settings**
* Default state for new SaaS businesses: **OFF**
* Changes take effect immediately after **Save**

**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049729631/original/c4U9EzbLVlpHLypPREqGmcFODpPs7OG9jg.png?1752242877)**

---

## **Manage Cancellation Reasons**

  
Collecting specific exit feedback helps you identify pricing objections, feature gaps, or onboarding challenges. Here you can configure a list of reasons that your clients will see when they attempt to cancel their SaaS subscription.  
  
To customize reasons:  
  
1. Go to **SaaS Configurator → Cancellation Settings**
2. Under **Manage Cancellation Reason**, choose from existing defaults or add new ones
3. Click the ✏️ icon to edit any listed reason or ➕ to add a new one
4. The **"Other"** option is always included and allows your customers to type a free-text response

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049081667/original/MsrKuMGjwHgpVQ80DEG8labRPshCYJaXRQ.png?1751285152)

---

## **Offer Discount to Retain Clients**

  
You can try to save the customer by offering a **discount** before they confirm cancellation. 

A well‑timed price break can nudge users to stay and explore more value before deciding. HighLevel automatically applies the coupon on the next billing cycle.  
  
To enable this:  
  
1. Toggle on **Enable Discount Offer**
2. Set:  
    
   * **Discount %** (e.g., 25%)  
   * **Discount Duration** (e.g., 3 months for monthly plans)
3. Optionally allow users to **receive the offer more than once**
4. When a customer accepts the offer, it’s **automatically applied** to their next billing cycle
5. Customers who accept will be **deflected** from cancellation

⚠️ This feature is currently available for **V1 sub-accounts only**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049081716/original/Y_1JJrodYvghRCvhvGPA942kM9SokSBePA.png?1751285182)

---

## **Redirect Users to an External Page**

  
If you want to handle cancellation logic outside the platform (e.g., on your own site), you can redirect users. This can be used for more advanced off-boarding flows, surveys, or saving attempts.  
  
Steps:  
  
1. Under **Redirect to External Page**, enter a valid URL
2. When enabled, users will be taken to this page immediately after selecting a cancellation reason
3. The cancellation will **not** complete within HighLevel

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049081726/original/-5esIHLnV47gNyPYzxPDy7xvKMNIN-H_mA.png?1751285207)

---

## **Track Cancellation Activity with Activity Logs**

  
All cancellation attempts are logged for visibility and analysis. This gives you actionable insights into **churn patterns** and **retention performance**.

  
To view logs:  
  
1. Scroll to the **Activity Logs** section
2. View:  
    
   * **Sub-account name & user**  
   * **Timestamp**  
   * **Plan details**  
   * **Cancellation reason**  
   * **Outcome (Cancelled / Deflected)**  
   * **Detection type** (e.g., coupon, redirect)
3. Use the **Download** button for exporting the log

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049081746/original/I-GIi7zy9SRof0upqSDhtKr5zKGvDSSQmQ.png?1751285223)

---

## **Preview the Cancellation Flow**

  
Before enabling the flow for your clients, you can simulate it using **Preview Mode**. Preview Mode reproduces the full client‑side journey in a safe sandbox, letting you double‑check copy, coupon math, and redirect destinations. No coupons are issued and no log entries are created while in Preview. This ensures a smooth and polished cancellation experience before going live.  
  
How to preview:  
  
1. Click **Preview** (top right of Cancellation Settings)
2. Navigate through each step as your customer would see it
3. Use this to validate text, offers, and logic flow

---

## **Frequently Asked Questions**

  
**Q: Can a client accept the discount more than once?**  
Yes. Check Allow Sub‑Accounts to receive discount offer more than once in Discount settings.  
  
**Q: What happens if I enable an external redirect and the user closes the browser?**  
The subscription remains active because the in‑app cancellation step was bypassed. The Activity Log will list Deflected – External Link.  
  
**Q: Where can I see which team member tried to cancel?**  
Check the User column in Activity Logs for the exact sub‑account admin.

  
**Q: Can I export the Cancellation Activity Log for auditing or reporting?**  
Yes. Click Download in Activity Logs to export a CSV that includes every cancellation and deflection event, along with reasons and user data.

  
**Q: Does Preview Mode create real coupons or log entries?**  
No. Preview runs in a sandbox environment. It displays the full flow for review but does not issue coupons, change subscription status, or write to Activity Logs.  

**Q: Are deflection events recorded even when the client ultimately keeps the subscription?**  
Yes. Activity Logs list every attempt, including deflections caused by discount acceptance or external redirect, so you always see total churn‑pressure volume.

---

## **Related Articles**

  
* [How to Cancel SaaS Sub‑Account for Your Client](https://help.gohighlevel.com/en/support/solutions/articles/48001216453)
* [Upgrading and Cancelling SaaS Plans for Clients](https://help.gohighlevel.com/en/support/solutions/articles/155000001979)
* [Subscription Management in Client Portal](https://help.gohighlevel.com/en/support/solutions/articles/155000003204)
* [Coupon Application on Subscription Products](https://help.gohighlevel.com/en/support/solutions/articles/155000004886)
* [Coupon Application on Subscription Products](https://help.gohighlevel.com/en/support/solutions/articles/155000004886)