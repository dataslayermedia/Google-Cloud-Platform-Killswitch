# Google-Cloud-Platform-Killswitch
 Add a limit on billing costs for your GCP account.

## Details from Google
https://cloud.google.com/billing/docs/how-to/notify



## Enable Budget Notifications

Navigate to Billing
Navigate to Budgets & alerts
CREATE BUDGET

## Listen to Notifications
Create a cloud function with trigger type Pub/Sub
Use the "index.js" and "package.json" scripts.
Swap out your project ID in the index.js file.



## Enable Cloud Billing API


## Service Account Upgrade
Provide Billing Administration access to the Cloud Function Service Account


## Publish Sub/Pub Message
https://console.cloud.google.com/cloudpubsub/topic/detail/budget-notifications?project=macgyver-services-production

```javascript
{
    "budgetDisplayName": "name-of-budget",
    "alertThresholdExceeded": 1.0,
    "costAmount": 100.01,
    "costIntervalStart": "2019-01-01T00:00:00Z",
    "budgetAmount": 100.00,
    "budgetAmountType": "SPECIFIED_AMOUNT",
    "currencyCode": "USD"
}
```

![Publish Test Message](https://raw.githubusercontent.com/tmoody/Google-Cloud-Platform-Killswitch/main/images/pub-sub-test-messaging.png)


## Validate that Billing is Disabled
https://console.cloud.google.com/billing/linkedaccount?project=macgyver-services-production

![Disabled Billing](https://raw.githubusercontent.com/tmoody/Google-Cloud-Platform-Killswitch/main/images/billing-disabled.png)

