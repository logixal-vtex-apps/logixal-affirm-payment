📢 Use this project, [contribute](https://github.com/vtex-apps/affirm-payment) to it or open issues to help evolve it using [Store Discussion](https://github.com/vtex-apps/store-discussion).

# Affirm Payment

This is a payment authorization app for the Affirm payment method (financing with monthly payments).

> ⚠️ _Currently Affirm cannot be used in a marketplace scenario where the seller processes the payment. In marketplace scenarios, the marketplace itself must process the payment._

## Configuration

1. Enable Affirm as a payment method in your store admin. In the Gateway Affiliation, enter your Affirm public API key as the `Application Key` and your Affirm private API key as the `Application Token`. For initial testing, set the Test/Production toggle to `Test` and use sandbox keys.
2. [Install this app](https://vtex.io/docs/recipes/development/installing-an-app/) in your account by running `vtex install vtex.affirm-payment`.
3. Configure the app settings by clicking `Apps > My Apps` in your account's admin sidebar and then selecting "Affirm Payment".

The available settings are:

- `Enable Katapult`: Katapult is a newer Affirm feature that offers a leasing option to shoppers who do not qualify for the normal Affirm financing. Please ask your Affirm contact to enable the feature on your Affirm account before enabling this app setting.
- `Company Name`: If you have multiple sites operating under a single Affirm account, you can override the external company/brand name that the customer sees. This affects all references to your company name in the Affirm UI. Leave blank to use your default company name stored in your Affirm account.
- `Public API Key for promotional components`: The public API key provided to you by Affirm.
- `Production Mode for promotional components`: Determines if the components from the [Affirm Components](https://github.com/vtex-apps/affirm-components) app run in Production or Sandbox mode.
- `Interval to use for the following three settings`: Determines the unit of time used by the following settings.
- `Delay to auto-settle`: Number of minutes/hours/days before authorized Affirm payments are automatically settled.
- `Delay to auto-settle after anti-fraud`: Number of minutes/hours/days before authorized Affirm payments are automatically settled after merchant's antifraud approval.
- `Delay to cancel`: Number of minutes/hours/days before Affirm payments are automatically canceled.
- `Katapult public token`: The public API token for your Katapult account. This is only needed if Katapult is enabled.
- `Katapult private token`: The private API token for your Katapult account. This is only needed if Katapult is enabled.
