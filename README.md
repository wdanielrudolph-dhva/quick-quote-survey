# Best Rate Shopper Survey Mockup

Standalone HTML/CSS/JavaScript version of the Dream House Virginia Best Rate Shopper survey, built to replace the GoHighLevel prebuilt Survey iframe while preserving the intended branching logic and field capture.

## Main File

- `brs-survey-mockup.html` contains the full standalone page.

## Current Status

- Standalone survey mockup is functional as a local HTML file.
- GoHighLevel submission is stubbed through `GHL_ENDPOINT`.
- GHL/contact/custom field names are centralized in `FIELD_MAP`.
- The page currently writes a draft payload to `window.bestRateShopperDraft` for inspection.

## Local Preview

Open `brs-survey-mockup.html` directly in a browser.

## GoHighLevel Connection Notes

When ready to connect:

1. Create or confirm matching GHL Contact/Object fields.
2. Update the keys in `FIELD_MAP`.
3. Set `GHL_ENDPOINT` to the chosen webhook or middleware endpoint.
4. Test each branch and inspect the payload before publishing.

## Core Branches

- Quote already received: captures interest rate and quoted loan amount.
- No quote + purchase: captures purchase details and calculates loan amount from purchase price and down payment.
- No quote + refinance: captures refinance loan amount.
- Financial details: captures estimated credit score, annual income, and available cash contribution.
- Contact details: captures full name, email, phone, and SMS consent.
