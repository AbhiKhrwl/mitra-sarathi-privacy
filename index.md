# Privacy Policy for Mitra Sarathi
**Effective Date:** July 3, 2026

Mitra Sarathi is committed to protecting your privacy. This policy explains how we handle user data. Our extension is designed with a privacy-first approach: all document formatting, cropping, and resizing operations are executed entirely on your local device.

---

## 1. Data Processing and On-Device AI
All image resizing, cropping, background removal, and document formatting are processed locally within your browser using WebAssembly (WASM). No images, documents, or personal files are ever uploaded, stored, or transmitted to any external server. Once you close the tab, all processed data is instantly cleared from the extension's memory.

---

## 2. Data We Collect and How We Use It
To manage premium tiers and usage quotas, we collect the following minimal information only if you choose to sign in:
* **Authentication and Identity:** If you log in via Google Identity (OAuth2), we receive your Google email address, name, and profile picture URL. This is used solely for account identification, premium plan verification, and daily quota reset management. We do not sell, rent, or share this data.
* **Telemetry and Usage Data:** Anonymous, non-personally identifiable operational metrics (such as performance indicators and error logs) may be collected to improve service stability.

---

## 3. Chrome Permissions Justification
Mitra Sarathi requests the following permissions strictly to enable its core features:
* **storage:** To save local preferences (such as auto-resize toggle state) and securely persist account session tokens locally.
* **identity:** To authenticate users via Google Sign-In for quota tracking and subscription tiers.
* **offscreen:** To run local image processing engines inside a secure DOM environment within Manifest V3.
* **notifications:** To show local alerts when you reach quota thresholds or when your plan is near expiration.
* **alarms:** To schedule periodic local checks for plan expiration.
* **host_permissions (http://*/*, https://*/*):** To inject the Drag-and-Drop formatting widget and read upload field dimensions on targeted portals where you upload files.

---

## 4. Third-Party Services
We utilize the following secure third-party infrastructure to operate the service:
* **Google Firebase:** For user authentication and quota database management.
* **Razorpay:** For processing secure payments and renewals.
* **Google Chrome Web Store API:** For delivering extension updates and validating license statuses.

---

## 5. Security Measures
We implement standard security measures, including HTTPS encryption for all authentication requests and strict Firebase Security Rules, to ensure your account data is protected. Because document processing is entirely local, the risk of document interception is eliminated by design.

---

## 6. Your Data Rights
You have the right to request a copy of the personal data we hold about you (your account profile) or request the permanent deletion of your account and associated database records.

---

## 7. Changes to This Privacy Policy
We may update this Privacy Policy from time to time to reflect changes in our practices or Chrome Web Store policies. We will notify you of any changes by updating the "Effective Date" at the top of this policy.

---

## 8. Contact Us
If you have any questions, concerns, or requests regarding this Privacy Policy or how your data is handled, please contact the developer at: [dev.abhishek.ai@gmail.com](mailto:dev.abhishek.ai@gmail.com)
