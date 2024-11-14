---
description: 3DS Decision Manager Setup
icon: screwdriver-wrench
---

# Setup Guide

{% hint style="info" %}
This section covers the steps to setup 3ds decision manager using the Superstream Control Center
{% endhint %}

## Steps to setup a rule on 3DS Decision Manager?

**Step 1:** Go to 3DS Decision Manager tab on the Superstream Control Center

**Step 2:** Click on create new rule&#x20;

**Step 3:** Save the rule name and description&#x20;

**Step 4:** Configure your desired rule by selecting the operators and values for the various fields&#x20;

**Step 5:** Add more rules using the plus icon on the top right of the current rule panel&#x20;

**Step 6:** Click save to configure and activate the rule&#x20;

**Step 7:** Your rule is now successfully configured and 3D Secure authentication would be enforced all payments conforming to this rule

**Note:** 3DS decision manager supports only one active configuration at a time. Multiple rules can be combined into a single configuration as shown in the example

### FAQs
<details>
<summary>What are some of the payment parameters that I can use to configure 3DS rules?</summary>

* **Amount** - Set rules for a specific value or a range of values for the transaction amount.
* **Currency** - Select the currency of the transaction.
* **Card Type** - Choose between credit and debit cards.
* **Card Network** - Choose between card networks like Visa, Mastercard, etc.
* **Billing Country** - Select the billing country.

</details>

<details>
<summary>How do I update the current configuration?</summary>
Click on Create New and configure a new rule that would replace the existing configuration
</details>

<details>
<summary>What happens if I set `authentication_type` as `three_ds` in `/payments` request?</summary>
3D Secure will be enforced and override the 3DS Decision Manager's decision
</details>