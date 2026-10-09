# Data Classification

**Status:** 🔴 RED — policy drafted; project data inventory pending.

## Purpose
Set handling requirements according to the sensitivity and impact of data.

## Default classes
- **Public:** intentionally published and approved for public access.
- **Internal:** non-public operational information with limited business impact if disclosed.
- **Confidential:** business-sensitive information, private correspondence, customer details, and non-public source artifacts.
- **Restricted:** passwords, API keys, access tokens, recovery codes, financial credentials, highly sensitive personal data, and data whose exposure could cause severe harm.

## Handling rules
- Collect and retain only what the product and approved purpose require.
- Grant access by least privilege and record sensitive access where appropriate.
- Do not commit secrets or restricted data to source control, prompts, test fixtures, or public logs.
- Redact data in examples, reports, screenshots, and support requests.
- Use approved transfer/storage channels and verify recipients before disclosure.
- Define retention, deletion, backup, and incident-response requirements.
- When classification is uncertain, handle data at the more protective level until clarified.

## Dependencies
Sections 03, 05, 09, and 11's secret/privacy/access controls.

## Acceptance evidence
A real project inventory assigns classes and handling rules to each material data category.

## Next action
Build the data inventory and map every class to storage, access, retention, and deletion controls.
