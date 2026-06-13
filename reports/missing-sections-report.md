# Missing sections report: payment gateway integration guides

This report audits integration guide pages under `/payments/payment-gateway/` for the following five required sections:

1. **Prerequisites** or "Before You Begin" section
2. **Step-by-step** integration instructions
3. **Code examples** (at least cURL + one SDK language)
4. **Test mode / sandbox** instructions
5. **Troubleshooting** or FAQ section

Priority is **High** if a page is missing 3 or more required sections, **Medium** if missing 1–2.

Each page is scored on its **own content only**. Hub pages that only link to subpages without including the relevant content themselves are marked as missing those sections, even if the content exists on a linked subpage.

## Summary

| # | Page | Missing sections | Priority |
|---|---|---:|---|
| 1 | `/payments/payment-gateway/quick-integration` | 4 | High |
| 2 | `/payments/payment-gateway/s2s-integration` | 4 | High |
| 3 | `/payments/payment-gateway/capacitor-integration` | 4 | High |
| 4 | `/payments/payment-gateway/cordova-integration` | 4 | High |
| 5 | `/payments/payment-gateway/zoho` | 4 | High |
| 6 | `/payments/payment-gateway/android-integration/standard` | 4 | High |
| 7 | `/payments/payment-gateway/android-integration/custom` | 3 | High |
| 8 | `/payments/payment-gateway/web-integration/standard` | 4 | High |
| 9 | `/payments/payment-gateway/web-integration/custom` | 3 | High |
| 10 | `/payments/payment-gateway/web-integration/hosted` | 4 | High |
| 11 | `/payments/payment-gateway/ios-integration/standard` | 4 | High |
| 12 | `/payments/payment-gateway/ios-integration/custom` | 4 | High |
| 13 | `/payments/payment-gateway/flutter-integration/standard` | 4 | High |
| 14 | `/payments/payment-gateway/flutter-integration/custom` | 3 | High |
| 15 | `/payments/payment-gateway/react-native-integration/standard` | 4 | High |
| 16 | `/payments/payment-gateway/react-native-integration/custom` | 3 | High |

## Details

### `/payments/payment-gateway/quick-integration`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/s2s-integration`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/capacitor-integration`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/cordova-integration`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/zoho`

- **Missing sections:**
  - Prerequisites / Before You Begin
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/android-integration/standard`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/android-integration/custom`

- **Missing sections:**
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/web-integration/standard`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/web-integration/custom`

- **Missing sections:**
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/web-integration/hosted`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/ios-integration/standard`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/ios-integration/custom`

- **Missing sections:**
  - Prerequisites / Before You Begin
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/flutter-integration/standard`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/flutter-integration/custom`

- **Missing sections:**
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/react-native-integration/standard`

- **Missing sections:**
  - Step-by-step integration instructions
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

### `/payments/payment-gateway/react-native-integration/custom`

- **Missing sections:**
  - Code examples (cURL + SDK)
  - Test mode / sandbox instructions
  - Troubleshooting / FAQ
- **Priority:** High

## Aggregate observations

- **Code examples (cURL + SDK)** are missing on **all 16** pages.
- **Test mode / sandbox** content is missing on **all 16** pages (most pages only reference a separate "Test integration" subpage as a step link).
- **Troubleshooting / FAQ** sections are missing on **all 16** pages (most reference a separate FAQ subpage via "Related information" links only).
- **Prerequisites** are present on 14 of 16 pages; missing on `zoho` and `ios-integration/custom`.
- **Step-by-step instructions** are present on 6 of 16 pages — all the **custom** variants (Android, Web, iOS, Flutter, React Native) and `zoho`, which use a `<Steps>` component. The **standard** and **hosted** variants and other top-level pages list only bullet links to subpages.
- All 16 pages are flagged **High** priority under the defined threshold (3+ missing sections).
