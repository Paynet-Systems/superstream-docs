---
icon: repeat
---

# Using Saved Payment Methods

Payment method details of users are stored in a secure PCI-compliant locker, for processing payouts in future. These stored payment method details can be listed for a given customer, which returns a `payment_token` for processing payouts.

### How does it work?

#### Persisting payment method details in a secure PCI-compliant locker

There are two entry points to storing payment methods for a given customer.

* Persisting payment methods prior to processing transactions
  * Payment methods can be created for a given customer using `/payment_methods` API.
  * This basically stores the passed payment method details in secure PCI-compliant locker.
* Persisting payment methods post a successful transaction
  * If a payment request was created with `"setup_future_usage": "off_session"` or if a payout request was created with `"recurring": true`, the payment method details will be stored in the secure locker once the transaction completes with a successful status.

#### Listing customer payment methods for processing payouts

Once the payment methods are stored in locker, they can be fetched using customer's list payment method API. This basically returns the identifiers for the saved payment methods along with a `payment_token` which can be used for processing transactions for a customer.

#### Processing payouts

Payouts can be created and processed using the `payment_token` for a given customer.

{% content-ref url="route-your-payout-transactions-using-smart-router.md" %}
[route-your-payout-transactions-using-smart-router.md](route-your-payout-transactions-using-smart-router.md)
{% endcontent-ref %}
