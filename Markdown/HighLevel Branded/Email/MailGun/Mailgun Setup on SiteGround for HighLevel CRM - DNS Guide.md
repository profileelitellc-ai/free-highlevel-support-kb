**Date Updated:** 2023-03-01T09:57:19.000Z

  
**TABLE OF CONTENTS**

* [Step-by-step Mailgun Setup - Siteground Domain Setup](#Step-by-step-Mailgun-Setup---Siteground-Domain-Setup)  
   * [To add the 1st TXT record](#To-add-the-1st-TXT-record)  
   * [To add the 2nd TXT record](#To-add-the-2nd-TXT-record)  
   * [To add the 1st MX records](#To-add-the-1st-MX-records)  
   * [To add the 2nd MX records](#To-add-the-2nd-MX-records)  
   * [To add the CNAME record](#To-add-the-CNAME-record)

  
# Step-by-step Mailgun Setup - Siteground Domain Setup

  
1\. Sign up for [Mailgun.com](https://signup.mailgun.com/new/signup)

  
2\. Check your email inbox to verify the email address

  
[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284378416/original/VewuZVN3oFOFIvBdf4XqMAOX4vtVGv_jNg.png?1677630998)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48243535009/original/7tQRdPUgguqaYEpnIV2uS3kIQpMd7jZBZw.png?1659724083)

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284378421/original/GU6IL6Y3N81qm6KMH9aTz7l5FV5IEv7ySA.png?1677630999)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48243535045/original/kRGmwZtbq3-zkULjp6-Pg0J-7sTNMNHymQ.png?1659724108)

  
3\. Login to Mailgun, Click on **Sending** \> **Add New Domain**

  
[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284378418/original/kxsnymCeuFAsBWkXaOes6QaaWED2_bfASA.png?1677630999)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48243535197/original/doBfy9jAqoxcOqD5LiuyQO9rnyVWfkkAeg.png?1659724186)
  
  
4\. If your domain is companyname.com, you can either set up the main domain or subdomain with Mailgun. 

  
A. Main domain:

* If you are adding the main domain,[ it should not be used with Gsuite, or any other email provider](https://help.mailgun.com/hc/en-us/articles/203357040-Can-I-Use-the-Same-Domain-Name-for-Mailgun-and-for-Google-Apps-Or-Another-Email-Server-)

 Subdomain:

* To set up the subdomain with Mailgun, you can type **ANYTHING\_HERE**.companyname.com  
   * Examples:  
         * mg.companyname.com  
         * replies.companyname.com  
         * support.companyname.com

B. Please set up the domain or subdomain under US, **not EU. not EU. not EU.** 

C. Click on **Add domain**

  
[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284382652/original/woVjMqNw3YY_Zjs20LoBHUb4KrThVvj_Rw.png?1677635102)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48243536037/original/B5DZocdO2h64MlEDtfuFjER-U%5F0AO%5FNOEg.png?1659724559)

  
The next screen that you're taken to will ask you to add DNS records to your domain. Leave this screen open for the next step.

  
![Screen Shot 2022-09-11 at 6.39.22 PM.png](https://help.mailgun.com/hc/article_attachments/8759612958491/Screen_Shot_2022-09-11_at_6.39.22_PM.png)

  
5\. Now log in to your DNS records based on where you get the domain and add the 5 DNS records.

##   

## To add the 1st TXT record

  
To [Add your first TXT record](https://world.siteground.com/kb/manage-dns-records/#TXT%5Frecord%5Fsettings), Log in to [](https://dash.cloudflare.com/login)[Siteground](https://login.siteground.com/login?lang=en)

Go to **Site Tools** \> **Domain** \> **DNS Zone Editor**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284391901/original/ZwLX5zPm5t6xvyGMrcxkIhoPH6U7XtbQsw.png?1677643178)

In the Create New Record section

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284392257/original/BnfApclXdbWZ_ONRoVqVaZZLCw-m9GTxFw.png?1677643477)

  
A. click on the **TXT** tab

  
B. Name: different for everyone, **DO NOT INCLUDE THE ROOT DOMAIN**

  
* Depending on the subdomain you are trying to set up, if you are trying to set up  
   * [mg.companyname.com](//mg.companyname.com) The host name will be **mg**  
   * [replies.companyname.com](//replies.companyname.com) The host name will be **replies**
* If you are setting up a **main** domain like companyname.com, the host name will be **@ or leave empty**

  
C. Value: Same for everyone

* paste the following record **v=spf1 include:mailgun.org \~all**
  
  
D. Click on Create

**![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284384681/original/QCbqi3BnzhNKNCspyADXNWBZfk3F55e2dg.png?1677636916)** 
  
  
## To add the 2nd TXT record

  
Click on **\+ Add Record** again

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284392423/original/WFBDHip6_j3WmEo4nRgIeENzQN-OEFhqqA.png?1677643605)
  
  
A. click on the **TXT** tab

  
B. Name: it's a bit tricky but the key here is to copy everything from the beginning until the subdomain part, **DO NOT INCLUDE THE ROOT DOMAIN**

  
**\*\*Everyone's 2nd TXT record host name and value is different**

  
Examples: copy the **highlighted part ONLY** and paste it in the Name field

| Example 1 using subdomain:Copy mx.\_domainkey.helpdesk as the host name | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284380215/original/t6MGY8Bw9AK1Vv01kUxtJAkNwp_4UfYjHw.png?1677632945) |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Example 2 using main domain:Copy mailo.\_domainkey as the host name     | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284380223/original/JSERXQQhYNvzVp7YoXhIji_yeomZNLXUKA.png?1677632951) |
  
  
C. Value: Head back to Mailgun and Copy and paste the 2nd TXT record here **highlighted in the screenshot below**

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284385043/original/UvAhE3LGN5sYkTb4kyEsXNM0GE0Uc8Eq1Q.png?1677637220)

  
D. Click on **Create**

  
## To add the 1st MX records

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284385538/original/qHcrrZPnp3g0LC4c75qM1hg_opwYUXgE0w.png?1677637720)  

  
Click on the **MX** tab > Select **Add your own MX records**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284392929/original/H-xERjs6rnHBgx2KfGgEYZBZ7Mmkxa_00A.png?1677644034)

  
If you have a Gsuite account to capture incoming emails for the main domain. Make sure you are using a subdomain for Mailgun. Check out [Can I Use the Same Domain Name for Mailgun and for Google Apps (Or Another Email Server)?](https://help.mailgun.com/hc/en-us/articles/203357040-Can-I-Use-the-Same-Domain-Name-for-Mailgun-and-for-Google-Apps-Or-Another-Email-Server-)
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284393043/original/KK8SevO7iTJJWSHB-9l9vRPfuZtGzkKxmw.png?1677644111)

  
A. Name: Different for everyone

  
Depending on the subdomain you are trying to set up, if you are trying to set up

* [mg.companyname.com](//mg.companyname.com) The Host Name will be **mg**
* [replies.companyname.com](//replies.companyname.com) The host Name will be **replies**

If you are setting up a **main** domain like companyname.com, the host name will be **@**

B. Priority is **10** which is also same for everyone no matter what domain you are trying to set

  
C. Destination: Same for everyone

 paste the following data **mxa.mailgun.org** 

  
D. Click on **Create**
  
  
## To add the 2nd MX records

  
Add another MX record again, this time Destination will be mx**_b_**.mailgun.org

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284393336/original/Rwlp0thYONnclsrwYeGKRE6xBW0jl1A2KQ.png?1677644328)

  
A. Name: Different for everyone

  
Depending on the subdomain you are trying to set up, if you are trying to set up

* [mg.companyname.com](//mg.companyname.com) The Host Name will be **mg**
* [replies.companyname.com](//replies.companyname.com) The host Name will be **replies**

If you are setting up a **main** domain like companyname.com, the host name will be **@**

B. Priority is **10** which is also same for everyone no matter what domain you are trying to set

  
C. Destination: Same for everyone

 paste the following data **mxb.mailgun.org**

  
D. Click on **Create**
  
  
## To add the CNAME record

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284385721/original/3LyKoigujZ-vEjMFQDflCfmRRfAJra3rYA.png?1677637907)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284393711/original/khGHMR_qTn12M2FmkiCTjNf8k9lHWO-gDw.png?1677644645)

  
A. Click on the **CNAME** tab

  
B. Name: Different for everyone

Head back to Mailgun to copy the host name, it's a bit tricky but the key here is to copy everything from the beginning until the subdomain part, **DO NOT copy the main domain**

  
Depending on the subdomain you are trying to set up, if you are trying to set up

* mg.companyname.com The host name will be **email** **.** **mg**
* replies.companyname.com The host name will be **email** **.** **replies**

If you are setting up a **main** domain like companyname.com, the host name will be **email**

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284385985/original/OtLw_A4zY8FbLbBKqMB9kUKRaQJO3xpp8A.png?1677638165)

  
C. Resolves to: Same for everyone

 paste the following data **mailgun.org**

  
D. Click on **Create**
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284393881/original/3o8rKOzJY89uxP0iayB1w-9flRZKZ1EM8g.png?1677644794)

Now that you have added 5 records, Go back to Mailgun and click on **Verify DNS Settings**
  
  
Click the same button to **Verify DNS Settings** again if some records are still not showing the green checkmark

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48284387965/original/I7T5QQCSjAnBvT1zqQlVgXSuNdgfuNiM3w.png?1677639928)
  
  
Once you add all the DNS records and verify, you can grab the [Mailgun API Key - Where to Find in Mailgun & Put in HighLevel](https://help.gohighlevel.com/en/support/solutions/articles/48000981682)

  
Then we could send a test email to see if everything works! Click here to learn [How to send a test email in the Conversation](https://help.gohighlevel.com/en/support/solutions/articles/48001208887)
  
  