---
description: Configure advanced rules with various payment parameters
icon: badge-check
---

# 3DS / Strong Customer Authentication

{% hint style="info" %}
Through this section, you will understand the working of 3DS Decision Manager and how to configure it.
{% endhint %}

Superstream 3DS Decision Manager allows the merchant to configure advanced rules using various payment parameters such as amount, currency etc., to enforce 3D Secure authentication for card payments to reduce fraudulent transactions.

## How does it work?

<figure><img src="../../../.gitbook/assets/final2.drawio.png" alt="" width="375"><figcaption><p>3DS Decision Flow</p></figcaption></figure>

* Superstream supports 3D Secure card payments via multiple payment processors
* The 3DS Decision Manager on the Superstream Control Center allows you to configure advanced rules based on payment parameters to decide when to enforce 3DS on card payments for supported processors
* For example, if you want to enforce 3DS authentication for all payments of value greater than $100 then you could setup the following rule on the 3DS Decision Manager and all the payment requests conforming to that rule would have `authentication_type` set as `three_ds`

<figure><img src="../../../.gitbook/assets/3ds-rule_example (1).png" alt=""><figcaption></figcaption></figure>

**Note:** If an explicit value is passed on `/payments` request using the `authentication_type` parameter it will override the 3DS Decision Manager - [API Reference](https://app.theneo.io/paynet/superstream)

Some payment processors mandate a 3D Secure authentication for all payments which will be enforced regardless of the `authentication_type` in `/payments` request

### Configure 3DS Decision Manager

Follow the [setup guide](setup-guide.md) to configure the 3DS Decision Manager