## Privacy Policy for Velo Sudoku

*Last updated: March 20, 2026*

> **Summary of changes (March 20, 2026):**
> - Section 2: Clarified that partner data is transmitted only after obtaining consent (not automatically).
> - Section 3B: Separated Firebase Analytics (Consent Mode v2 / TCF) from Crashlytics and Performance (separate consent). Added information about cookieless pings.
> - Section 3C: Added Google Play Services (payments).
> - Section 5: Added ability to delete individual statistics entries and manage consents in app settings.
> - Section 6: Expanded consent mechanisms description: CMP (IAB TCF v2.2) for ads and analytics, separate form for crash reports and performance data.

### 1. Introduction
This privacy policy explains how data is processed and protected in the **Velo Sudoku** mobile application (hereinafter "App"). We respect user privacy and are committed to transparency regarding the technologies used.

### 2. Data, Permissions and No Backend
The App does not have its own backend server and does not transmit personal user data to the Developer. We do not require account creation, login, or providing a name or email address.

The App processes data in the following ways:
* **Local Processing:** Game progress, settings, puzzle solving times, and statistics are stored exclusively in the secure internal memory of the user's device.
* **Third-Party Processing:** The App uses external libraries (SDKs) that may collect device identifiers and diagnostic data, only after obtaining explicit User consent. No personal data or device identifiers are transmitted to partners before consent is given. The only exception is anonymized, identifier-free measurement data (so-called cookieless pings) that Google Firebase may send as part of the Consent Mode v2 mechanism — details in section 3B.

### 3. Third-Party Partners and Data Sharing
We have integrated trusted third-party services with the App. We do not have direct access to data collected by these systems.

**A. Google AdMob (Advertising)**
Ad provider. May use device identifiers for ad personalization.
* **Consent:** Personalized ads are displayed only after consent is given in the CMP (Consent Management Platform) window compliant with the IAB TCF v2.2 standard. Without consent, ads may be displayed in non-personalized form.
* Google Privacy Policy: https://policies.google.com/privacy

**B. Google Firebase (Analytics, Stability and Performance)**
The App uses three Firebase services that are subject to **separate consent mechanisms**:

1. **Firebase Analytics (usage statistics):**
   * Analytics consent (`analytics_storage`) is managed by a CMP compliant with the IAB TCF v2.2 standard and mapped to **TCF Purpose 1** ("Store and/or access information on a device").
   * At app startup, all Consent Mode v2 signals (analytics_storage, ad_storage, ad_user_data, ad_personalization) are set to **DENIED** by default.
   * **Cookieless pings:** Even without user consent, Google Firebase may send anonymized measurement data without device identifiers (so-called cookieless pings) as part of the Consent Mode v2 mechanism. This data does not contain information that could identify the user and is used solely for statistical modeling.
   * After consent is given in the CMP, signals are updated to GRANTED, enabling full analytics data collection.

2. **Firebase Crashlytics (crash reports) and Firebase Performance (performance data):**
   * These are managed by a **separate consent mechanism**, independent of the CMP and TCF.
   * Upon first app launch, an introductory form is displayed where the User decides whether to enable crash and performance reporting.
   * Without this consent, Crashlytics and Performance are completely disabled — no reports are sent.
   * The User can change this decision at any time in the App Settings ("Privacy" section).

* Firebase Privacy Policy: https://firebase.google.com/support/privacy

**C. Google Play Services (Payments)**
The App uses Google Play services for in-app purchases. The Developer does not have access to the User's financial data.

### 4. Purpose of Actions
The actions taken by the App are intended for:
1. **Game Functionality:** Saving game state (Save/Load) — local data.
2. **Maintenance and Development:** Monitoring crashes and statistics — only with User consent.
3. **Monetization:** Displaying ads — personalized only with User consent.

### 5. Data Deletion
Full control over data lies with the User.

**Managing Game Progress (Local Data):**
* **Deleting individual entries:** The User can manually delete selected results in the Statistics section.
* **Complete data deletion:** To permanently delete all progress, uninstall the app or clear its data (*Android Settings -> Apps -> Velo Sudoku -> Storage -> Clear Data*).

**Managing Consents (External Data):**
The User can withdraw or change their consents at any time in the App Settings ("Privacy" section):
* **Ad and analytics consent** — by reopening the CMP form.
* **Crash report and performance consent** — via the toggle in settings.
Withdrawing consent will immediately stop the transmission of relevant data to partners.

**Advertising Data (Google):**
The User can additionally reset their advertising identifier in device settings:
* *Android Settings -> Google -> Ads -> Reset advertising ID* or *Delete advertising ID*.
* To manage data associated with your Google account, visit: https://myactivity.google.com/

### 6. GDPR (User Consent)
Under the GDPR, users in the European Economic Area (EEA) and the United Kingdom have full rights to decide about their data.

The App uses **two separate consent collection mechanisms:**

1. **CMP Form (Consent Management Platform):**
   * Displayed on first app launch, compliant with the **IAB TCF v2.2** standard.
   * The User decides on consent for **personalized advertising** and **analytics** (TCF Purpose 1).
   * Consents for advertising (`ad_storage`, `ad_user_data`, `ad_personalization`) and analytics (`analytics_storage`) are **independent** of each other — the User can accept one without the other.
   * The CMP form can be reopened in the App Settings ("Privacy" section).

2. **Introductory Form (Crash reports and performance):**
   * Displayed on first launch, separately from the CMP.
   * The User decides whether to enable **Firebase Crashlytics** (crash reports) and **Firebase Performance** (performance data).
   * This decision can be changed at any time in the App Settings.

If the User does not give consent:
* No personal data or device identifiers will be sent to Google Firebase or AdMob.
* Google Firebase may only send anonymized cookieless pings as part of Consent Mode v2, which do not contain data that could identify the user.

### 7. Contact
For privacy policy inquiries, please contact us at:
**minigamesforeveryone@gmail.com**

*Note: To facilitate a quick response regarding privacy matters, please include "Privacy" or "GDPR" in the subject line of your email.*
