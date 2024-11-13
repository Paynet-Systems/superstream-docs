---
description: >-
  This section offers an outline of the best practices implemented within the
  Superstream cloud environment, aimed at ensuring a secure, user-friendly, and
  efficiently managed platform
icon: id-card-clip
---

# Identity and Access Management

## Authentication Methodology for Superstream APIs

### Admin Services Authentication:

Administrative services, crucial for managing the back end of Superstream, are protected using multi-layered authentication mechanisms. Access to the admin services involves an additional API key, restricted to a select few individuals with the Superstream team.

### Merchant Authentication:

For merchants accessing Superstream, we have a strong authentication mechanism to ensure the confidentiality and integrity of their accounts.

### Vault Authentication:

Superstream Vault has a security setup where key custodians are in charge of managing distributed keys. To start the vault application, all these key custodians must work together.&#x20;

The design ensures that no single custodian possesses the capability to independently tamper with the vault application, enhancing the overall security of the system.

## Identity and Access Management in AWS

### User Authentication:

Superstream employs a robust authentication methodology for users, ensuring secure access to the platform. Users are authenticated by Multi-Factor Authentication combined with network and device-level whitelisting

### Access Controls and RBAC:

Access controls in Superstream are finely tuned through Role-Based Access Control (RBAC). Distinct administrative roles are defined, each with granular permissions tailored to specific responsibilities. This ensures that users, admins only have access to the resources and functionalities necessary for their roles.

#### Admin Role:

Superstream operates on a distributed access model, ensuring that no individual possesses complete administrative control.

#### Limiting Permissions:

Superstream empowers administrators to limit permissions effectively. Through the IAM (Identity and Access Management) module, access policies are crafted following the Principle of Least Privilege. This means that each user, admin is granted the minimum permissions necessary to perform their tasks, minimizing the risk of unauthorized access.
