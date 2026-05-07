---
layout: default
title: Privacy Policy - Mitra Sarathi
---

# Privacy Policy for Mitra Sarathi

**Effective Date:** April 24, 2026

Mitra Sarathi ("we," "our," or "us") is highly committed to protecting your privacy and ensuring the absolute security of your documents. This Privacy Policy explains how our Chrome Extension collects, uses, and safeguards your information. We have designed Mitra Sarathi with a strict **Privacy-First** architecture to ensure your sensitive data remains on your device.

---

## 1. Data Processing and On-Device AI

Our core functionality involves formatting, resizing, and cropping images, specifically highly sensitive documents like passports, signatures, and government IDs. 

**All image processing, background removal, and facial detection occur entirely locally on your device** within your browser's secure environment using WebAssembly (WASM) technology.

*   **No Cloud Uploads:** We **do not** upload, store, transmit, or back up your images or documents to any external servers. 
*   **Zero Knowledge:** We **do not** have access to the personal data contained within your processed files. Once you close the tab or inject the image into a form, the localized data is instantly cleared from the extension's memory.

## 2. Data We Collect and How We Use It

To provide, maintain, and secure the Mitra Sarathi service, we collect the following minimal data:

### 2.1. Authentication and Identity
Mitra Sarathi offers an optional login feature using Google Chrome Identity (OAuth2) via Firebase Authentication to manage usage quotas and premium tiers.
*   **What we collect:** If you choose to log in, we collect basic profile information strictly limited to your **Email address, Name, and Profile Picture URL**.
*   **How we use it:** This data is used solely for account identification, quota management, and to provide customer support.
*   **Data Sharing:** We **do not** sell, rent, or share this personal information with any third parties or data brokers under any circumstances.

### 2.2. Telemetry and Usage Data
To improve the extension and maintain system reliability, we may collect anonymous, non-personally identifiable operational data.
*   **What we collect:** Aggregated operational metrics (e.g., number of images processed, error logs, quota threshold events).
*   **How we use it:** To monitor system health, fix bugs, and understand feature adoption. This data **cannot** be traced back to your actual documents, portal activity, or web browsing history.

## 3. Chrome Permissions Justification

Mitra Sarathi requires specific Chrome permissions to function seamlessly. We adhere to the principle of least privilege. Here is exactly why we request these permissions:

*   **`identity`**: Required to allow users to securely log in via Google OAuth2. This powers our user authentication and allows us to seamlessly manage your usage quotas and premium access tiers without requiring you to create a separate password.
*   **`storage`**: Used to save your local extension preferences (e.g., your auto-resize toggle state) and to securely persist Firebase authentication tokens locally so you remain logged in across sessions.
*   **`activeTab` & `scripting`**: Required to dynamically inject the Mitra Sarathi Drag-and-Drop overlay UI directly into the web form you are currently viewing. This is essential for the extension to programmatically insert the processed, final images directly into the website's file input fields, saving you manual effort.

## 4. Third-Party Services

We utilize the following trusted third-party infrastructure to operate Mitra Sarathi:
*   **Google Firebase:** Used securely for user authentication and quota database management.
*   **Google Chrome Web Store API:** Used for securely authenticating identity and delivering extension updates.

## 5. Security Measures

We implement industry-standard security measures, including HTTPS encryption for all authentication requests and strict Firebase Security Rules, to ensure your account data is protected against unauthorized access. Because document processing is entirely local, the risk of document interception is fundamentally eliminated by design.

## 6. Your Data Rights

Depending on your region (and in compliance with frameworks like the DPDP Act), you have the right to:
*   Request a copy of the personal data we hold about you (your account profile).
*   Request the permanent deletion of your account and associated database records.
*   Opt-out of optional communications.

To exercise any of these rights, please contact us using the information below.

## 7. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in our practices or Chrome Web Store policies. We will notify you of any significant changes by updating the "Effective Date" at the top of this policy.

---

## 8. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy or how your data is handled, please contact the developer at:

**Email:** dev.abhishek.ai@gmail.com
  

