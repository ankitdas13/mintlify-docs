# Missing Sections Report: Payment Gateway Integration Guides

This report audits integration guide pages under `payments/payment-gateway/` for the following required sections:

1. **Prerequisites** — A "Prerequisites" or "Before You Begin" section.
2. **Step-by-step integration instructions** — Numbered or clearly enumerated steps.
3. **Code examples** — At least one cURL example AND at least one SDK language example (Node, Java, Ruby, Python, PHP, Go, Kotlin, Swift, .NET).
4. **Test mode / sandbox instructions** — Guidance on testing in sandbox / test mode (test cards, `rzp_test` keys, test integration, etc.).
5. **Troubleshooting or FAQ section** — A troubleshooting and/or FAQ section.

For pages with a corresponding subdirectory of MDX files (e.g. `web-integration/standard.mdx` + `web-integration/standard/*.mdx`), the audit considers content across the page and its subpages as one guide.

**Priority:** High if 3 or more sections are missing, Medium if 1–2 sections are missing.

## Pages with missing sections

| Page path | Missing sections | Priority |
| --- | --- | --- |
| `payments/payment-gateway/s2s-integration/redirect.mdx` | Troubleshooting/FAQ | Medium |
| `payments/payment-gateway/ecommerce-plugins/arastta.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/bigcommerce.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/build-your-own.mdx` | Prerequisites | Medium |
| `payments/payment-gateway/ecommerce-plugins/cs-cart.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/drupal-commerce.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/easy-digital-downloads.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/gravity-forms.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/magento.mdx` | Code examples (missing SDK language) | Medium |
| `payments/payment-gateway/ecommerce-plugins/open-cart.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/prestashop.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/shopify.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/shopify-cod.mdx` | Prerequisites, Code examples (cURL + SDK), Troubleshooting/FAQ | High |
| `payments/payment-gateway/ecommerce-plugins/shopify-razorpay-secure.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/whmcs.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/wix.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/woocommerce.mdx` | Code examples (cURL + SDK) | Medium |
| `payments/payment-gateway/ecommerce-plugins/wordpress.mdx` | Code examples (missing cURL) | Medium |
| `payments/payment-gateway/zoho.mdx` | Prerequisites, Code examples (cURL + SDK), Test mode/sandbox, Troubleshooting/FAQ | High |

## Pages with all required sections

The following pages contain all five required sections (covering the landing page and its subpages where applicable):

- `payments/payment-gateway/web-integration/standard.mdx`
- `payments/payment-gateway/web-integration/custom.mdx`
- `payments/payment-gateway/web-integration/hosted.mdx`
- `payments/payment-gateway/android-integration/standard.mdx`
- `payments/payment-gateway/android-integration/custom.mdx`
- `payments/payment-gateway/ios-integration/standard.mdx`
- `payments/payment-gateway/ios-integration/custom.mdx`
- `payments/payment-gateway/flutter-integration/standard.mdx`
- `payments/payment-gateway/flutter-integration/custom.mdx`
- `payments/payment-gateway/react-native-integration/standard.mdx`
- `payments/payment-gateway/react-native-integration/custom.mdx`
- `payments/payment-gateway/capacitor-integration.mdx`
- `payments/payment-gateway/cordova-integration.mdx`
- `payments/payment-gateway/quick-integration.mdx`
- `payments/payment-gateway/s2s-integration.mdx`

## Notes on methodology

- Detection uses keyword/pattern matching on combined page + subpage content:
  - Prerequisites: matches `prerequisite`, `before you begin`, `before you start`.
  - Step-by-step: matches `step <n>`, `integration step`, `steps to integrate`, or presence of an `integration-steps` subpage.
  - cURL: matches fenced code blocks starting with `curl` / `bash` containing `curl`, or inline `curl -X` patterns.
  - SDK language: matches fenced code blocks with language tags `node`, `nodejs`, `javascript`, `js`, `java`, `ruby`, `python`, `php`, `go`, `kotlin`, `swift`, `csharp`, `dotnet`.
  - Test mode/sandbox: matches `test mode`, `sandbox`, `test integration`, `test card`, `test key`, `rzp_test`, `test environment`.
  - Troubleshooting/FAQ: matches `troubleshoot`, `faq`, `frequently asked`.
- For e-commerce plugin guides, "code examples" typically aren't applicable because integration is performed via plugin install/UI configuration rather than API calls. These are flagged for completeness per the audit criteria; reviewers may choose to mark them as not-applicable.
- The report covers primary integration guide landing pages. Sub-feature pages (e.g. `web-integration/custom/chargeback.mdx`) are not audited individually.
