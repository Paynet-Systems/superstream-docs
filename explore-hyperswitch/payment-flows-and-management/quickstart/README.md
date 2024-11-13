---
description: Start accepting one time payments with Superstream in 4 easy steps
icon: bolt
---

# Accept Payments

{% hint style="info" %}
This section gives you the steps to get started with Superstream, configure your payment processor, integrate with your application and accept your first payment in minutes
{% endhint %}

## Getting Started

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th><th data-hidden data-card-cover data-type="files"></th></tr></thead><tbody><tr><td><strong>Quickstart guide</strong></td><td>Integrate Superstream from scratch and accept your first payment in minutes</td><td></td><td><a href="./#get-your-hyperswitch-api-key">#get-your-hyperswitch-api-key</a></td><td><a href="../../../.gitbook/assets/quickstart.jpg">quickstart.jpg</a></td></tr><tr><td><strong>Migrate from Stripe</strong></td><td>Already a Stripe user? Learn how you can quickly migrate to Superstream</td><td></td><td><a href="migrate-from-stripe/">migrate-from-stripe</a></td><td><a href="../../../.gitbook/assets/StripeMigration.jpg">StripeMigration.jpg</a></td></tr><tr><td><strong>Payment recipes</strong></td><td>Explore quick payment recipes consisting of combinations of use case specific payment processors</td><td></td><td><a href="payment-recipes/">payment-recipes</a></td><td><a href="../../../.gitbook/assets/recipe.jpg">recipe.jpg</a></td></tr></tbody></table>

## Get your Superstream API key

If you have not created a sandbox account, please create one

If you have already created a sandbox account, your api key could be fetched from settings section.

## Configure your payment processor

Configure the payment processor of your choice using Connectors tab on our control center. You will need to have the API credentials of the payment processor readily available.

If you do not have access to the API credentials of your payment processor, do not worry. Superstream has a demo payment processor automatically configured to your sandbox account. It will assist you to simulate various payment flows and assist you in completing the integration.

## Integrate Superstream

Don't want to write code? Check out the [Superstream Postman Collection](https://app.theneo.io/paynet/superstream/superstream-api-documentation) for a no-code way to get started with Superstream's API.

You will be using both a server and a client-side component of Superstream to complete the integration.

The payment flow begins once your user has added products to a shopping cart and now wishes to make a payment.

**Step 1:** Your server will create a payment with Superstream server, to get a client\_secret.

**Step 2:** Your website loads and initiates the [Superstream SDK](../../merchant-controls/integration-guide/) to render a payment widget to the customer. Depending on the customer's currency and country, the list of payment methods are displayed to the customer.

**Step 3:** The customer chooses a payment method, enters additional information (say card details) and hits the pay button.

**Step 4:** Superstream SDK securely transmits the payment information to Superstream Server. The Superstream server processes the payment with the most suitable payment processor, as per the your smart routing algorithm.

**Step 5:** Upon successful payment, the customer is automatically redirected to your payment status confirmation page.

<figure><img src="../../../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>

## Configure and manage payment methods on the Superstream Control Center

The control center provides complete control on your payment operations.

* **Enable and manage payment processors:** Easily onboard multiple payment processors and manage payment methods with a few clicks.
* **Track payment and refund information:** The unified control center allows you to query upon a particular payment or refund. You may also initiate refunds from the control center.
* **Smart payment routing:** You will have the complete capability to dynamically set the payment routing logic based on 20+ variables. Use this to optimize your payment processing goals.

<details>

<summary>FAQs</summary>

#### What is a connector?

Superstream refers to payment processors, fraud / risk engines and other payment integrations as connectors. Superstream currently supports 50+ global payment processors that you can use to process payments on your application

#### How can I decide the best payment methods for my business?

Superstream supports 100+ payment methods across various payment processors. There is no one size fits all payment methods but you can learn more about how you can decide the best payment methods for you business [here](payment-methods-setup/).

#### What will the completed integration look like?

Superstream offers various customization options but you can try out our demo store [here](https://demo-hyperswitch.netlify.app/checkout) to test the checkout experience

#### Are there any sample integrations for reference?

Here are a few demo integrations for various tech stacks:

* [Hyperswitch React-Node](https://github.com/juspay/hyperswitch-react-node)
* [Hyperswitch HTML-Node](https://github.com/juspay/hyperswitch-html-node)
* [Hyperswitch React-Java](https://github.com/juspay/hyperswitch-react-java)
* [Hyperswitch Next-Node](https://github.com/juspay/hyperswitch-next-node)



</details>
