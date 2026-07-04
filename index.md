# Privacy Policy for Mitra Sarathi

**Effective Date:** July 4, 2026  
**Last Updated:** July 4, 2026  
**Version:** 3.0  
**Developer:** Mitra Sarathi Team  

---

## 1. Introduction

Mitra Sarathi ("the Extension", "we", "our", "us") is an AI-powered browser extension that provides intelligent document formatting, image optimization, and file processing assistance for web-based form submissions. This Privacy Policy explains how we collect, use, protect, and handle information when you use our Extension.

By installing or using Mitra Sarathi, you agree to the practices described in this Privacy Policy. If you do not agree, please uninstall the Extension.

---

## 2. Information We Collect

### 2.1 Information You Provide Directly

- **Account Information:** When you sign in using Google Authentication (via Chrome's built-in identity system), we receive your Google account email address and display name solely for account identification, subscription management, and personalized usage analytics.
- **Feedback Data:** If you voluntarily submit feedback through the Extension, we collect your star rating, improvement suggestions, and issue descriptions.
- **Referral Data:** If you participate in our referral programme, we store anonymized referral codes linked to your account.

### 2.2 Information Collected Automatically

- **Usage Metrics:** We collect aggregate, non-identifiable processing statistics such as total images processed, document types handled, and feature utilization frequency. These metrics help us improve our proprietary optimization algorithms and deliver personalized usage insights within the Extension.
- **Subscription Status:** Your active plan tier (Free, PRO, or ULTRA) and associated quota consumption data are stored to enforce fair-use limits and deliver appropriate service levels.
- **Extension Configuration:** Your preferences, including auto-resize settings, blocked website lists, and notification preferences, are stored locally using Chrome's Storage API.

### 2.3 Information We Do NOT Collect

- **Images and Documents:** We do not collect, upload, transmit, store, or access the content of any images, photographs, documents, or files you process through the Extension. All file processing operations are executed exclusively within your browser's local runtime environment.
- **Form Data:** We do not read, capture, or transmit any form field values, personal identification information, or government document data from any website you visit.
- **Browsing History:** We do not track, record, or monitor your browsing activity, visited URLs, or navigation patterns.
- **Keystroke Data:** We do not log keystrokes, clipboard contents, or text input on any page.

---

## 3. How We Process Your Data

### 3.1 On-Device Processing Architecture

Mitra Sarathi employs a proprietary multi-stage processing pipeline that executes entirely within your browser's sandboxed environment. Our technology stack includes:

- **Proprietary AI Models:** Our neural network models for face detection, document boundary analysis, and intelligent content classification run locally using WebAssembly (WASM) and ONNX Runtime within an isolated offscreen processing context.
- **Adaptive Image Optimization Engine:** Our proprietary algorithms for format conversion, resolution scaling, compression optimization, and aspect ratio enforcement operate exclusively in-browser using hardware-accelerated Canvas APIs.
- **Intelligent Context Analysis System:** Our proprietary heuristic engine analyzes form field metadata (HTML attributes, labels, and validation rules) to determine optimal output parameters. This analysis reads only structural page metadata — never user-entered content.
- **Background Removal Engine:** Powered by our integrated AI segmentation models operating in an isolated WebAssembly sandbox with zero network dependency.

This architecture ensures that your sensitive documents and personal photographs never leave your device during processing operations.

### 3.2 Cloud Services

The following cloud services are used for non-processing functions only:

- **Google Firebase Authentication:** For secure user identity verification and session management.
- **Google Cloud Firestore:** For storing account-level metadata (subscription status, usage quotas, referral data). No user files or processed content are stored in any cloud database.
- **Razorpay Payment Gateway:** For processing subscription payments. Payment transactions are handled entirely by Razorpay's PCI-DSS compliant infrastructure. We do not store credit card numbers, CVV codes, or banking credentials.
- **Google Cloud Functions:** For server-side subscription validation, referral code generation, and payment webhook processing.

### 3.3 Remote Camera Assistance (Optional Feature)

Mitra Sarathi includes an optional Remote Camera feature that enables real-time video assistance between two parties using peer-to-peer WebRTC technology. When activated:

- Video streams are transmitted directly between participants using encrypted peer-to-peer connections (DTLS-SRTP). No video data passes through or is stored on our servers.
- WebRTC signaling metadata (connection establishment parameters only) is temporarily exchanged via Firebase Firestore and is automatically purged after the session ends.
- This feature is entirely user-initiated and requires explicit activation. It is never activated automatically.

---

## 4. Permissions Justification

Mitra Sarathi requests the following browser permissions, each essential for core functionality:

| Permission | Purpose |
|-----------|---------|
| **storage** | Stores your preferences, processing quota counters, blocked website list, and session state locally on your device using Chrome's Storage API. No data is synced externally through this permission. |
| **identity** | Enables secure Google Sign-In through Chrome's built-in identity system for account authentication and subscription management. No third-party authentication libraries are used. |
| **offscreen** | Creates an isolated background processing context for running AI models (face detection, background removal, document analysis) without blocking your active browsing. This is required for WebAssembly execution in a separate thread. |
| **notifications** | Delivers smart usage alerts (approaching daily processing limits), subscription renewal reminders, and monthly usage summaries. Notifications are rate-limited and respect system Do Not Disturb settings. |
| **alarms** | Schedules periodic background checks (every 6 hours) for delivering timely quota and subscription alerts. No user data is accessed during these checks. |
| **Host Permissions (all URLs)** | Content scripts must be available on any website to detect file upload form fields and provide universal image optimization assistance. The Extension monitors only `<input type="file">` elements and associated form metadata — it does not read page content, inject advertisements, or modify non-file-related page elements. Users can disable the Extension on any specific website using the built-in Blacklist feature. |

---

## 5. Data Storage and Security

### 5.1 Local Storage
Extension preferences, processing statistics, and configuration data are stored locally on your device using Chrome's encrypted Storage API. This data never leaves your browser unless you explicitly sign in to sync subscription-related metadata.

### 5.2 Cloud Storage Security
Account metadata stored in Firebase Firestore is protected by:
- Firebase Security Rules enforcing per-user data isolation (users can only access their own records)
- TLS 1.3 encryption for all data in transit
- AES-256 encryption for data at rest
- Strict access control policies limiting server-side access

### 5.3 Payment Security
All payment processing is handled by Razorpay, a PCI-DSS Level 1 certified payment processor. We never receive, process, or store your payment card details. Subscription status is communicated to our system via secure server-to-server webhooks.

---

## 6. Data Retention and Deletion

- **Local Data:** All locally stored data (preferences, cache, processed image buffers) can be instantly cleared by uninstalling the Extension or clearing browser data. Processed images exist only in volatile memory during the active processing session and are never persisted.
- **Account Data:** Your account metadata (email, usage stats, subscription status) is retained while your account is active. You may request complete deletion of your account data by contacting us at the email below.
- **Payment Records:** Transaction records are maintained by Razorpay according to their data retention policy and applicable financial regulations.
- **Feedback Data:** Voluntarily submitted feedback is retained for product improvement purposes and can be deleted upon request.

---

## 7. Data Sharing and Third-Party Disclosure

We do not sell, trade, license, or rent your personal information to any third party.

We share limited data only with the following service providers, solely for the purposes described:

| Provider | Data Shared | Purpose |
|----------|------------|---------|
| Google Firebase | Email, display name | Authentication, account management |
| Razorpay | Transaction metadata | Payment processing |
| Google Cloud Functions | Account ID | Subscription validation, referral processing |

We may disclose information if required by law, legal process, or governmental request, or to protect the rights, safety, or property of our users or the public.

---

## 8. Children's Privacy

Mitra Sarathi is not directed to children under the age of 13. We do not knowingly collect personal information from children. If you are a parent or guardian and believe your child has provided personal information, please contact us to request deletion.

---

## 9. Your Rights

Depending on your jurisdiction, you may have the following rights:

- **Access:** Request a copy of the data we hold about you.
- **Correction:** Request correction of inaccurate account data.
- **Deletion:** Request deletion of your account and associated data.
- **Data Portability:** Request your data in a machine-readable format.
- **Withdrawal of Consent:** Uninstall the Extension at any time to cease all data processing.
- **Objection:** Object to specific data processing activities by contacting us.

To exercise any of these rights, please contact us using the information below.

---

## 10. International Data Transfers

Account-level metadata may be processed and stored on servers located outside your country of residence, including in the United States (Google Cloud infrastructure) and India (Razorpay infrastructure). By using the Extension, you consent to the transfer of your account metadata to these jurisdictions. All transfers are protected by the security measures described in Section 5.

---

## 11. Intellectual Property and Proprietary Technology

Mitra Sarathi's AI models, optimization algorithms, heuristic engines, context analysis systems, and processing pipeline architecture are proprietary and confidential. The Extension's on-device processing capability does not imply that any proprietary algorithms, model weights, training data, or trade secrets are disclosed, licensed, or made available for inspection, reverse engineering, or competitive analysis. All intellectual property rights are expressly reserved.

---

## 12. Updates to This Policy

We may update this Privacy Policy from time to time to reflect changes in our practices, technology, legal requirements, or for other operational reasons. The updated policy will be posted at this URL with a revised "Last Updated" date. Continued use of the Extension after any changes constitutes acceptance of the updated policy.

---

## 13. Cookie Policy

Mitra Sarathi does not use cookies, tracking pixels, web beacons, or any other tracking technologies. We do not participate in any advertising networks or cross-site tracking programmes.

---

## 14. Open Source Components

Mitra Sarathi incorporates certain open-source software components licensed under their respective open-source licenses. The use of these components does not affect the proprietary nature of our custom algorithms, AI models, and processing pipeline.

---

## 15. Limitation of Liability

Mitra Sarathi is provided "as is" without warranties of any kind. We are not responsible for any data loss, corruption, or damage arising from the use of the Extension. Users are advised to maintain independent backups of important documents before processing.

---

## 16. Governing Law

This Privacy Policy shall be governed by and construed in accordance with the laws of India, without regard to its conflict of law provisions.

---

## 17. Contact Information

For questions, concerns, data deletion requests, or to exercise your privacy rights, please contact:

**Developer:** Mitra Sarathi Team  
**Email:** dev.abhishek.ai@gmail.com  
**Extension:** Mitra Sarathi (AI-Powered Form Assistant)

---

*This privacy policy is designed to comply with the Chrome Web Store Developer Program Policies, the Google API Services User Data Policy, the EU General Data Protection Regulation (GDPR), the California Consumer Privacy Act (CCPA), and India's Digital Personal Data Protection Act, 2023 (DPDPA).*
