---
description: >-
  Automatically retry failed non-3DS payments by stepping them up to 3DS
  authentication
icon: angles-up
---

# 3DS Step-up Retries

{% hint style="info" %}
This section covers how 3DS Step-up retries function, the supported payment processors, and how to enable it.
{% endhint %}

3DS Step-up Retries is a Superstream feature designed to enhance non-3DS payment success rates. If a non-3DS payment fails and we detect a relevant error message suggesting the potential for improved success with 3DS authentication, we seamlessly step up the authentication and attempt the payment again with same payment processor to increase the likelihood of a successful transaction.

**3DS Step-up retries:** These retries are applicable when errors are identified in non-3DS payments that can be resolved by attempting 3DS authentication. Examples of errors that can be addressed through 3DS authentication include, but are not limited to, fraud-related errors and 3DS authentication-required errors.

## How does it work?

The flow looks like the following:

<figure><img src="../../../.gitbook/assets/Screenshot 2023-12-07 at 5.56.20 PM.png" alt=""><figcaption></figcaption></figure>

## Supported Payment processors

Superstream supports the following processors for 3DS Step-up retries.

* Bluesnap
* Stripe

## How to enable 3DS Step-up retries?

Drop a request to biz@Superstream.io with confirmation to enable 3DS Step-up retry

### FAQs

<details>

<summary>What will the user experience look like during 3DS Step-up Retry?</summary>

The user experience will slightly differ in this flow because, when we step up the authentication to 3DS, user involvement is required to provide extra authentication, which is typically not the case in non-3DS payments.

</details>

<details>
<summary>What is the difference between Smart retry and 3DS Step-up retry?</summary>

While Smart Retry attempts both to retry all the eligible business and technical failures with an alternative processor, 3DS Step-up Retry primarily addresses failures that can be easily eliminated by stepping up the authentication. This approach increases the payment success rate, enabling the business to relax regarding chargeback liability.

</details>

<details>
<summary>What if the failure is eligible for both 3DS Step-up retry and Smart retry?</summary>

If a non-3DS payment failure is eligible for both types of retries, we choose to proceed with 3DS Step-up Retry. We attempt the payment by enforcing 3DS authentication with the same processor, as this reduces chargeback cases and ensures the transaction is not fraudulent.&#x20;

</details>