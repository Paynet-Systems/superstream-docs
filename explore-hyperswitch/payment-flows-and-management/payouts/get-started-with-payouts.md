---
icon: flag-checkered
---

# Get started!

For getting started with payouts, make sure you have signed up for the underlying payout processors supported by Superstream.

## How does it work?

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

## How to get started?

We will be using Superstream's hosted dashboard and Postman API collection for configuring connectors and processing payouts. You can find API reference [here](https://app.theneo.io/paynet/superstream/payouts).

#### Pre-requisites

* Make sure you have an account by signing up at the dashboard.
* Log in to the dashboard
* Make sure you have an API key by navigating to _**Developers**_ section
* Note down your `merchant_id` from the home page.

#### Steps for configuring payout processors

**Step 1 -** Login to your Superstream account.

**Step 2** - Navigate to _**Payout Processors**_ tab.

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Payout Processors list</p></figcaption></figure>

**Step 3 -** Select the payout processor you'd want to use and provide the processor's credentials.

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Configuring auth keys for communicating with the processor</p></figcaption></figure>

**Step 4 -** Enable preferred payment methods.

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Keep preferred payment methods enabled</p></figcaption></figure>

**Step 5 -** Hooray! You've successfully set up your payout processor!

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Successfully configured!</p></figcaption></figure>

#### Steps for processing payouts

**Step 1 -** Import postman collection from [here](https://www.postman.com/hs-payouts/hyperswitch/collection/u6uep7u/payouts-w-hyperswitch).

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Import postman collection</p></figcaption></figure>

**Step 2 -** Navigate to _**Variables**_ tab to set up below variables

* `baseUrl`
* `merchant_id`
* `api_key`

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Updating env variables in postman collection</p></figcaption></figure>

**Step 3 -** Head to "Process payouts" section for processing payouts.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-10-18 at 12.10.26 PM.png" alt=""><figcaption></figcaption></figure>

{% content-ref url="process-payouts-using-saved-payment-methods.md" %}
[process-payouts-using-saved-payment-methods.md](process-payouts-using-saved-payment-methods.md)
{% endcontent-ref %}
