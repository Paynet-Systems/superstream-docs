---
icon: swap
---

# Smart Router for Payouts

**Note: routing rules are distinct for payment and payout operations. Configuring one does not affect the other and vice-versa.**

## How to get started?

Routing rules can be configured using Superstream's dashboard _(beta feature)_ or via APIs. We will be using Superstream's dashboard as it provides a simple, intuitive UI for configuring these rules.

#### Pre-requisites

Make sure there are at least two or more payout processors integrated with your account.

#### Steps for configuring routing rules for payouts

**Step 1 -** Head to _**Workflow -> Payout Routing**_

**Step 2 -** From here, you can select one of the three routing rule formats for creating a routing rule and follow one of the below guides for configuring your routing rule

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-cover data-type="files"></th></tr></thead><tbody><tr><td></td><td>Volume Based Routing</td><td></td><td><a href="../../../.gitbook/assets/image (12).png">image (12).png</a></td></tr><tr><td></td><td>Rule Based Routing</td><td></td><td><a href="../../../.gitbook/assets/image (13).png">image (13).png</a></td></tr><tr><td></td><td>Default fallback Routing</td><td></td><td><a href="../../../.gitbook/assets/image (14).png">image (14).png</a></td></tr></tbody></table>

**Step 3 -** You can view the created routing rules at the main page

**Step 4 -** Only a single routing rule can be activated at a given time. For selecting a different rule, click on the rule and click `Activate Configuration`

**Step 5 -** If none of the rules are activated, the transaction is routed in the order listed in Default Fallback Priority