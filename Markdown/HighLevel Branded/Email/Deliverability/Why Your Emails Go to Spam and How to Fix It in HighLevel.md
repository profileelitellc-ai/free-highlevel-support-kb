**Date Updated:** 2025-07-23T20:59:12.000Z

The article addresses common reasons why emails sent through HighLevel might end up in spam folders. It highlights factors such as poor sender reputation, lack of proper authentication (like SPF and DKIM), and content issues (like spammy keywords or formatting). The article provides actionable tips to improve email deliverability, including verifying domain settings, maintaining a clean email list, and monitoring engagement metrics. By following these guidelines, users can enhance their email marketing effectiveness and reduce the chances of their emails being marked as spam.

---

**TABLE OF CONTENTS**

* [Sending From a Public Domain](#Sending-From-a-Public-Domain)
* [DMARC](#DMARC)
* [List Health & List Collection](#List-Health-&-List-Collection)
* [Sending Internal Mail](#Sending-Internal-Mail)
* [Frequently Asked Questions](#Frequently-Asked-Questions)
* [Related Articles](#Related-Articles)

---

There are many reasons that mailbox providers could flag your email as spam. Here are the most common reasons we see and how to fix them!

  
## **Sending From a Public Domain**

  
If you are sending messages from a free domain like gmail.com, yahoo.com, etc., your messages will likely go to the spam folder. You'll want to be sure to send mail from a domain that you own and that matches your branding.  
  
**Check out our guide on** - [Dedicated Email Sending Domains Overview & Setup](https://help.gohighlevel.com/en/support/solutions/articles/48001226115)

---

## **DMARC**

  
If the domain you use to send mail has a DMARC policy but you haven't verified the domain in with your SMTP provider, your messages will likely go to spam. Check with your SMTP provider for instructions on how to ensure your HighLevel messages pass DMARC.

---

## **List Health & List Collection**

  
If all of the technical pieces above are covered, list health and list collection are the next most important factors to determine deliverability. Be sure that:

  
* Everyone on your list gave direct consent to receive email marketing from you
* Your cold subscribers are cleaned from your list regularly
* Your forms are secured with double opt-in

  
To learn more about why messages go to the inbox or spam folder, check out our [Introduction To Email Deliverability](https://help.gohighlevel.com/en/support/solutions/articles/48001063371) article.

---

## **Sending Internal Mail**

  
Are you sending messages to the same domain that the message is coming from? For example, sending from info@exampledomain.com to suan@exampledomain.com. If so, it's common for these internal messages to go to spam. This is because your mailbox sees that it's receiving a message from itself, but it knows that it didn't send the message (HighLevel did). This makes your mailbox think it's being spoofed, and it sends the message to spam.

  
If you're just sending internal mail to test your messages, we recommend using a free email like gmail.com. If you need to send mail internally outside of testing, you'll want to have the person who manages mail for your domain whitelist the IP address of your SMTP provider.

---

## **Frequently Asked Questions**

  
**Q: How can I test if my emails are going to spam before sending them to my list?**

You can use email testing tools that analyze your email content and sender reputation. Additionally, consider sending test emails to different email providers (like Gmail, Yahoo, etc.) to see where they land.

  
**Q: What steps can I take if my domain has a poor sender reputation?**

Improving your domain's sender reputation involves several strategies, including gradually increasing your email sending volume, regularly cleaning your email list, and actively engaging with your audience to boost open rates.

  
**Q: How often should I clean my email list to avoid spam issues?**

It's recommended to clean your email list every 6 to 12 months. Regularly remove inactive subscribers and those who haven't engaged with your emails to maintain a healthy list and improve deliverability.

---

## **Related Articles**

  
* [Email Sending Guide: Email Best Practices & Email Warm Up](https://help.gohighlevel.com/en/support/solutions/articles/155000001021)
* [What is LC Email?](https://help.gohighlevel.com/en/support/solutions/articles/48001220605)
* [What is a dedicated IP in LC email?](https://help.gohighlevel.com/en/support/solutions/articles/155000001152)
* [An Introduction To Email Deliverability](https://help.gohighlevel.com/en/support/solutions/articles/48001063371)
* [How to use the Email Risk Assessment Tool for LC Email](https://help.gohighlevel.com/en/support/solutions/articles/155000000577)