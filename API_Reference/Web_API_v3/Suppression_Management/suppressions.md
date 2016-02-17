---
layout: page
title: Suppressions
weight: 80
navigation:
  show: true
---

Suppressions are email addresses that can be added to [groups]({{ root_url }}/API_Reference/Web_API_v3/Suppression_Management/groups.html) to prevent certain types of emails from being delivered to those addresses.

{% anchor h2 %}
POST
{% endanchor %}

Add recipient addresses to the suppressions list for a given group.

{% info %}
If the group has been deleted, this request will add the address to the global suppression.
{% endinfo %}

{% parameters post %}
  {% parameter recipient_emails Yes 'Array of valid email addresses' 'Addresses to add to the suppression group' %}
{% endparameters %}

{% apiv3example post POST https://api.sendgrid.com/v3/asm/groups/:group_id/suppressions recipient_emails=['test1@example.com','test2@example.com'] %}
{% v3response %}
HTTP/1.1 201
{"recipient_emails":["test1@example.com","test2@example.com"]}
{% endv3response %}
{% endapiv3example %}

* * * * *

{% anchor h2 %}
GET
{% endanchor %}

Get suppressed addresses for a given group.

{% apiv3example get GET https://api.sendgrid.com/v3/asm/groups/:group_id/suppressions %}
{% v3response %}
HTTP/1.1 200
["test1@example.com","test2@example.com"]
{% endv3response %}
{% endapiv3example %}

* * * * *

{% anchor h2 %}
DELETE
{% endanchor %}

Delete a recipient email from the suppressions list for a group.

{% apiv3example get DELETE https://api.sendgrid.com/v3/asm/groups/:group_id/suppressions/:email_address %}
{% v3response %}
HTTP/1.1 204
{% endv3response %}
{% endapiv3example %}
