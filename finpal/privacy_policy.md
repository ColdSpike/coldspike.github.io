# Privacy Policy for FinPal

**Last updated:** October 30, 2026

This Privacy Policy describes how FinPal ("we", "us", or "our") collects, uses, and discloses your information when you use our mobile application ("App").

## 1. Information We Collect

### A. SMS Data (Financial Transactions)
FinPal requests access to your SMS messages solely for the purpose of automatically tracking your income and expenses.
*   **What we access:** We scan your SMS inbox for transaction-related messages (e.g., from banks, credit cards, or mobile wallets).
*   **How it is processed:** SMS processing uses the on-device parser by default.
*   **Local SMS records:** Transaction and review records can contain the original SMS and sender. Gatekeeper Analytics also keeps local filtering logs, including original text for new logs, so you can inspect why a message was allowed or rejected. Filtering logs older than 30 days are removed when new filtering logs are recorded. These local records are not automatically synchronized to a cloud transaction database.
*   **Optional AI Processing:** Users with active Premium access, including the 30-day trial, may explicitly enable cloud AI parsing. When enabled, selected transaction messages are masked and sent with the message timestamp and the names of available categories and financial accounts to FinPal's Google-hosted processing service, which uses Google Gemini. Masking reduces exposure but does not guarantee that all identifying details are removed. Turning this setting off stops future cloud parsing. Cloud AI access stops when the trial expires unless lifetime Premium is purchased.

### B. Personal Information
*   **Account Info:** When you sign in with Google or email and password, Firebase Authentication processes your sign-in information. We use your account identifier, email address, available display name, profile-photo URL and last-login timestamp to manage your account and Premium status. Signing in is optional for local expense tracking.
*   **Trial Eligibility:** We store server-generated trial start and end timestamps and whether the one-time trial was claimed for your authenticated account.
*   **Financial Data:** Your transaction history, budget, and categories are stored locally on your device.

### C. Device Information
Firebase Remote Config downloads configuration used by the SMS filters and parser. It uses Firebase installation identifiers and technical service information; this can occur even if you do not sign in. Google Play and Firebase also process device, network and account information needed for authentication, purchases, configuration delivery and service security. FinPal's Google-hosted backend may produce operational request and error logs. Local app diagnostic logs can also be stored on your device.

### D. Optional Attachments, Backups and Support
Receipt images you attach are stored locally. If you export an encrypted backup, you choose where to save the file and are responsible for its password and any copies. FinPal does not automatically upload receipt images or backup files to its backend. If you contact us or submit a deletion request, we receive the contact information and content you choose to provide; please do not send passwords, OTPs or full banking credentials.

## 2. How We Use Your Information

We use the information we collect to:
1.  **Provide Features:** Automatically generate transaction records from your bank SMS.
2.  **Manage Accounts:** Verify your identity, enforce one trial per account, and sync your Premium access across devices.
3.  **Protect Services:** Authenticate requests and prevent abuse of optional cloud services.

FinPal does not display advertising or use your SMS content for advertising. The app does not include Firebase Analytics or Firebase Crashlytics. SMS processing is used for expense tracking, categorization, review and related budgeting features.

## 3. Third-Party Services

We use the following third-party services, which may collect information used to identify you:
*   **Google Sign-In:** For authentication.
*   **Google Play Services:** For In-App Purchases and license verification.
*   **Firebase (Google):** For authentication, cloud profiles, Premium/trial records and Remote Config.
*   **Google Gemini through Vertex AI:** For optional cloud SMS parsing after explicit consent.

Cloud requests use HTTPS. Cloud AI payloads may include transaction amounts, merchants, dates and custom category/account labels as well as the masked message. These requests can be processed outside your country, including through Google's global AI endpoint. Our parser does not intentionally write SMS prompts and responses to its application database. Google's service-side safety, abuse-monitoring, caching and operational retention practices can still apply; we do not promise anonymous processing or zero retention. See [Firebase privacy and security](https://firebase.google.com/support/privacy) and [Google Cloud's generative-AI data controls](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/vertex-ai-zero-data-retention).

## 4. Your Controls, Retention and Deletion

* **SMS and cloud processing:** You can revoke SMS permission in Android settings. Starting a trial, upgrading to Premium or restoring Premium enables the AI tracking preference. Before sending SMS to the cloud, FinPal asks for your explicit consent on that device if you have not already given it for the signed-in account. You can choose Not now to continue with on-device tracking. You can disable Cloud AI transaction tracking in FinPal Settings; this stops future cloud processing, and ordinary membership checks do not switch it back on. Without SMS permission, automatic SMS tracking and inbox imports are unavailable, but manual entry remains available.
* **Local records:** Transactions, budgets, accounts, categories and attached receipts remain on your device unless you choose to export or back them up. Manually deleted transactions remain in the local Recycle Bin for up to 30 days; active Premium or trial access is required to restore them. Expired items are removed when FinPal next performs its cleanup. Wipe All Data permanently clears the app's local records. Copies you exported or backed up must be deleted separately.
* **Account deletion:** Signed-in users can choose Settings → Delete Account. After identity verification, this deletes the Firebase sign-in account and cloud profile. It does not delete local financial records; use Wipe All Data separately if desired. If you no longer have the app, use the [FinPal Account Deletion Request form](https://docs.google.com/forms/d/e/1FAIpQLSfMbO7k-T3JCmUoJt4bkGHv9_Osi7AA3lzp7YdqJ27Brs6A_Q/viewform) or email **[support@finpal.makp.in](mailto:support@finpal.makp.in?subject=FinPal%20account%20deletion)** with the subject **FinPal account deletion**. Identify the email address used for your FinPal account. We may verify ownership before acting. You do not need to reinstall the app to request deletion.
* **Service records:** Limited server-side entitlement, purchase-verification and trial-eligibility records are stored separately from the cloud profile and retained to verify ownership, restore valid purchases and prevent fraud or repeated free trials. They include one-way hashes of provider identifiers, verified email addresses or account identifiers, trial dates, account identifiers and purchase tokens. They do not preserve your deleted cloud profile. Contact us with requests concerning these records.
* **Purchases and trials after deletion:** Google Play handles payments; FinPal does not receive your payment-card details. Account deletion does not refund or cancel a lifetime purchase. To restore a valid purchase, sign back in with the same Google account, use the Google Play account that bought Premium, then open Premium in Settings and choose Restore Previous Purchases. Purchases whose access has been revoked cannot be restored. Refund eligibility is governed by Google Play's policies and applicable law. Deleting or recreating an account does not pause or restart the one-time trial; the original expiry date remains in effect.
* **Other data requests:** You may email us to request deletion of data without deleting your sign-in account. Specify what you want removed. We will explain any information that must be retained for purchase verification, security or abuse prevention. Removing FinPal's local records does not remove messages from your phone's SMS inbox, and account deletion does not by itself request a Google Play refund.

## 5. Contact Us

If you have any questions about our Privacy Policy, contact us at **[support@finpal.makp.in](mailto:support@finpal.makp.in)**.
