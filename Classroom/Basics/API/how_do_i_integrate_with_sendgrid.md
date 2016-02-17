---
seo:
  title: How do I Integrate with SendGrid?
  description: How do I Integrate with SendGrid?
  keywords: marketing, webhook, newsletter, getting, started, whitelabel, getting_started, email, api, integration, smtp, what, warm
title: How do I Integrate with SendGrid?
weight: 0
layout: page
zendesk_id: 200182018
navigation:
  show: true
---

There are many&nbsp;different ways to use SendGrid’s email services so it all comes down to what&nbsp;_you_&nbsp;need. We have numerous examples for how to configure mail clients such as Outlook and Apple Mail to send through our system as well as integration examples for a multitude of programming languages and libraries on our&nbsp; [SendGrid Integration Page](http://sendgrid.com/docs/Integrate/index.html).

**The main ways you can integrate with Sendgrid:&nbsp;**

- [SMTP]({{root_url}}/Classroom/Basics/Email_Infrastructure/what_is_smtp.html)&nbsp;- Send using a desktop mail client, or existing program/service with [your smtp credentials]({{root_url}}/Classroom/Basics/Email_Infrastructure/recommended_smtp_settings.html).&nbsp;
- [Web API](https://sendgrid.com/docs/API_Reference/Web_API/index.html)&nbsp;- Send from your app using&nbsp; [your api key]({{root_url}}/Classroom/Basics/API/what_is_my_api_key.html). Check out our [API Guide](http://go.sendgrid.com/rs/sendgrid/images/SendGrid_API_Guide-101.pdf) for more info.
- [Email Marketing App and API](https://sendgrid.com/docs/User_Guide/Legacy_Features/Marketing_Emails/index.html)&nbsp;- Send from our content creation UI and manage your lists via the website.&nbsp;

&nbsp;

**Things to consider before you start sending:**

- We recommend that all users complete [Whitelabeling]({{root_url}}/Classroom/Deliver/Delivery_Introduction/all_you_need_to_know_about_whitelabeling.html) for their accounts. This process helps your emails look as legitimate as possible!
- Also consider implementing the&nbsp; [Event API](http://sendgrid.com/docs/API_Reference/Webhooks/event.html)&nbsp;to track and log your email data more thoroughly. For more info on the benefits of Event API, check out our&nbsp; [_Why Event API_]({{root_url}}/Classroom/Basics/API/why_event_api.html)&nbsp;article. The Event API is available to all account levels except for Lite.
- We _**highly**_ recommend that if you are a Silver or&nbsp;higher customer, you [warm up your IP](https://sendgrid.com/docs/User_Guide/warming_up.html) as part of your getting started checklist. Warming up is one of the best ways to prevent delivery issues down the road!

&nbsp;
