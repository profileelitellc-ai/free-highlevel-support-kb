**Date Updated:** 2025-03-11T20:40:13.000Z

A digital check-in and ticketing system allows businesses to manage customer visits, offers, and campaigns efficiently. This article provides a step-by-step guide on setting up a digital check-in system in HighLevel, enabling businesses to generate QR-coded tickets, track redemptions, and automate workflows.

  
**TABLE OF CONTENTS**

* [Key Benefits of a Digital Check-In System](#Key-Benefits-of-a-Digital-Check-In-System)
* [Step 1: Setting Up the Check-In Form](#Step-1%3A-Setting-Up-the-Check-In-Form)
* [Step 2: Generating Prefilled URLs for Each Customer](#Step-2%3A-Generating-Prefilled-URLs-for-Each-Customer)
* [Step 3: Creating a Trigger Link for Better Tracking](#Step-3%3A-Creating-a-Trigger-Link-for-Better-Tracking)
* [Step 4: Sending QR Codes via Email](#Step-4%3A-Sending-QR-Codes-via-Email)
* [Step 5: Automating the Check-In Process](#Step-5%3A-Automating-the-Check-In-Process)
* [Step 6: Preventing Multiple Redemptions](#Step-6%3A-Preventing-Multiple-Redemptions)
* [Frequently Asked Questions](#Frequently-Asked-Questions)

  
---
  
  
---

## **Key Benefits of a Digital Check-In System**

A digital check-in system streamlines customer engagement and enhances business operations. Key benefits include:

* **Automated QR Code Generation**: Each customer receives a unique ticket.
* **Efficient Tracking**: Staff can verify ticket eligibility instantly.
* **Pre-filled Check-In Forms**: Reduces manual data entry.
* **Redemption Control**: Prevents multiple uses of the same offer.
* **Automated Review Requests**: Encourages feedback collection.
* **Customizable for Different Use Cases**: Ideal for restaurants, events, and promotions.

---

## **Step 1: Setting Up the Check-In Form**

A check-in form collects customer information and confirms ticket validity when scanned by staff.

1. **Go to Sites** in your HighLevel sub-account.
2. Navigate to **Forms > Builder** and click **Add Form**.
3. Select a **restaurant-related template** to save time.
4. Customize the form by:  
   * Keeping essential fields: **Full Name, Phone Number, Email**.  
   * Removing unnecessary fields.  
   * Renaming the submission button to **Check-In**.
5. **Add a custom field:**  
   * Click **Add Element** and create a **Single Line** field.  
   * Name it **Redeem Status** and group it under **Contact**.  
   * Save and **hide** this field (it will store ticket redemption info).
6. Click **Save Form**.

---

## **Step 2: Generating Prefilled URLs for Each Customer**

Prefilled URLs ensure that when a customer scans a QR code, their information is automatically filled in.

1. **Save your form** and click **Integrate** to copy the form link.
2. Modify the URL structure to prefill data dynamically:  
   * Use query parameters to pass customer details:  
   ```  
   ?full_name=Contact.Name&phone=Contact.Phone&email=Contact.Email&redeem_status=False  
   ```  
   * Ensure consistency so that existing customer details match HighLevel records.
3. Save this modified link for use in QR code generation.

---

## **Step 3: Creating a Trigger Link for Better Tracking**

Trigger links shorten and track URL clicks, allowing workflow automation.

1. Go to **Marketing > Trigger Links**.
2. Click **Add Link** and name it accordingly (example: Free Dessert Campaign)
3. Paste the modified URL (from Step 2) and save it.

---

## **Step 4: Sending QR Codes via Email**

Each customer receives a unique QR code linked to their personal check-in form.

1. **Use API.QRServer.com** to generate QR codes dynamically.
2. Create an **email template**:  
   * Add campaign details and instructions.  
   * Insert the same **image header** as the form.  
   * Use the following structure for dynamic QR code generation:  
   ```  
   https://api.qrserver.com/v1/create-qr-code/?data=<<TRIGGER_LINK>>  
   ```  
   * Replace `<<TRIGGER_LINK>>` with the actual trigger link.
3. Test the email by sending it to yourself and scanning the QR code.

---

## **Step 5: Automating the Check-In Process**

Ensure a smooth workflow by automating customer check-ins and redemption tracking.

1. **Create a workflow:**  
   * Navigate to **Automations > Workflows** and click **Create Workflow**.  
   * Set the **trigger** to **Form Submitted** and select your check-in form.  
   * Add the following actions:  
         * **Add a Tag**: `Free Dessert Checked-In`.  
         * **Update Contact Field**: Set `Redeem Status` to `True`.  
         * **Send a Review Request** (optional).  
         * **Log Data to Google Sheets** (optional for tracking check-ins).
2. **Publish and Save** the workflow.

---

## **Step 6: Preventing Multiple Redemptions**

To prevent customers from using the same QR code multiple times:

1. **Modify the check-in form:**  
   * Go to **Sites > Forms** and open the form.  
   * Click **Conditional Logic** and add a rule:  
         * **If Redeem Status = True**, **Disqualify the lead**.  
         * Show a message: "You’ve already redeemed this ticket. Thank you for your visit."  
   * Save the form.
2. **Test by scanning twice:**  
   * First scan should allow check-in.  
   * Second scan should show a disqualification message.  
   * Verify in **Form Submissions** that only one successful submission exists.

---

## **Frequently Asked Questions**

### **Q: Can I use this system for events instead of restaurants?**

Yes! This system works for events, workshops, and other campaigns where unique ticketing is required.

### **Q: How do I track which customers redeemed the offer?**

You can track redemptions through **Form Submissions** or **Google Sheets Integration**.

### **Q: Can I customize the email template further?**

Absolutely! Modify the email content and QR code placement as needed.

### **Q: What happens if a customer tries to redeem a ticket twice?**

The system prevents duplicate redemptions by checking the `Redeem Status` and disqualifying them.

### **Q: How do I add SMS notifications for staff members?**

Use the **Workflow Automation** feature to send SMS notifications when a check-in occurs.

---

## **Related Articles**

* How to Create and Manage Forms in HighLevel
* Using Trigger Links for Campaign Tracking
* How to Automate Email Campaigns in HighLevel
* Creating Custom Fields for Better CRM Management

---

## **Next Steps**

1. Set up your **check-in form** following the instructions.
2. Generate **dynamic QR codes** and test email delivery.
3. Automate **workflows for check-in tracking** and redemption control.
4. Ensure **duplicate redemption prevention** is working correctly.
5. Monitor results and optimize your campaign.

This guide provides a structured way to implement a digital check-in system in HighLevel, ensuring smooth ticketing and campaign tracking. If you have questions, feel free to reach out!
  
  