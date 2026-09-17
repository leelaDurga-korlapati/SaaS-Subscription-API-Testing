# SaaS-Subscription-API-Testing
   PayPal Sandbox API testing for SaaS subscription Workflow

## Overview
API testing project simulating a SaaS subscription billing workflow using PayPal Sandbox APIs.

## What I Did

### Authorization
- Generated an OAuth access token using PayPal Sandbox Client ID and Secret.

### Products
- Created a product using the Catalog Products API.
- Tested product listing using GET.
- Tested product update using PATCH.
- Attempted DELETE and confirmed that the Product API does not support this method.
- Tested error scenarios including 400 (Bad Request), 401 (Unauthorized), and 404 (Not Found).

### Plans
- Created a billing plan linked to a product.
- Accidentally created an additional plan during testing and deactivated it.
- Verified that the plan was deactivated.
- Tested error scenarios including 400 (Bad Request), 401 (Unauthorized), and 404 (Not Found).

### Subscriptions
- Created a subscription using the billing plan.
- Approved the subscription through the PayPal Sandbox approval flow.
- Verified that the subscription became ACTIVE.
- Tested an invalid subscription ID and received a 404 (Not Found) response.
- Created another subscription and cancelled it.
- Verified the cancellation.

## Tools Used
- Postman (API testing)
- PayPal Developer Sandbox (testing environment)
