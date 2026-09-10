## Privacy Policy for Velo Sudoku

*Last updated: September 10, 2026*

> **Summary of changes (September 10, 2026):**
> - Section 2: Added a description of in-game reminders — they are created solely on the device, require consent (system permission and an in-app switch), can be turned off in Settings, and carry no advertising content.
> - Section 4: Added gameplay reminders to the list of purposes.

> **Summary of changes (August 25, 2026):**
> - Section 3D: Widened the scope of data copied to Play Games cloud save — besides statistics and resources, the copy now also carries game settings and notification preferences, the crash-reporting consent, the accepted version of the legal documents, and challenge progress (daily, weekly and monthly puzzles, including make-up days). Clarified that advertising consents (CMP/TCF) are **not** copied and stay on the device.
> - Section 2: Clarified that Android Auto Backup also covers the App's settings, excluding advertising consents.

> **Summary of changes (August 11, 2026):**
> - Section 2: Corrected the description of data storage — beyond the device's memory, data may be copied to the User's own Google account (Android's automatic app backup, and cloud save once the game is connected to Play Games). The Developer still has no backend server and no access to these copies.
> - Section 3D: Added Google Play Games Services (cloud save) — scope of copied data, the optional nature of connecting, turning it off and deleting the copy.
> - Section 5: Added management of cloud copies (deleting the Play Games copy, Android's automatic app backup).

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
* **Local Processing:** Game progress, settings, puzzle solving times, and statistics are stored in the secure internal memory of the user's device.
* **Copies on the User's Google account:** Two mechanisms may additionally copy this data **to the User's own Google account** — never to the Developer, who has no backend server and no access to these copies: **Android's automatic app backup** (the system "Auto Backup for Apps" feature, which copies app data and settings to the User's Google Drive — excluding advertising consents, which stay on the device; unrelated to Android Auto) and, once the game is connected to **Google Play Games**, **cloud save** (see section 3D).
* **Third-Party Processing:** The App uses external libraries (SDKs) that may collect device identifiers and diagnostic data, only after obtaining explicit User consent. No personal data or device identifiers are transmitted to partners before consent is given. The only exception is anonymized, identifier-free measurement data (so-called cookieless pings) that Google Firebase may send as part of the Consent Mode v2 mechanism — details in section 3B.
* **Notifications (in-game reminders):** The App may display reminders about the User's daily streak, about the daily puzzle, and reminders to come back after a longer break. Notifications are created **solely on the User's device** — their content is not sent to the Developer or to any third party, and the App uses no server for this purpose. Delivery requires the User's consent: the system permission (Android 13 and later) and a switch inside the App. Consent can be withdrawn at any time — in the system settings or in **Settings → Notifications**. Reminders contain no advertising or commercial offers.

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

**D. Google Play Games Services (Cloud Save)**
Once the game is connected to Google Play Games, the User's progress is additionally saved to their Play Games profile ("Saved Games"), inside Google's infrastructure and linked to their Google account. This keeps progress available when changing phones or reinstalling the game.

* **Connecting is optional:** The App never forces sign-in. Silent sign-in happens only if the User has previously enabled automatic sign-in for games in their Google Play Games settings. Otherwise no data is sent until the User taps "Connect" in the App Settings.
* **Scope of copied data:** game statistics, best streak, streak freezes, in-game resources, challenge progress (completed daily, weekly and monthly puzzles together with the make-up state), as well as game settings and notification preferences, the crash- and performance-reporting consent, and the accepted version of the legal documents. Purchases are **not** part of this copy — they are restored by Google Play billing. **Advertising consents (CMP/TCF) are not copied either** — they stay on the device, so the User makes that choice again on a new phone.
* **Data received from Play Games:** the player ID and the Play Games display name. These are used solely to show which profile the game is connected to. The Developer still has no backend server, no access to the User's Google account, and no way to read these copies outside the device.
* **Turning it off:** *App Settings -> Cloud backup -> "Save progress" toggle*. New progress stops being saved immediately.
* **Deleting it:** *App Settings -> "Delete cloud copy"*. Play Games data for this game — or the entire Play Games profile — can also be deleted directly at Google: https://support.google.com/googleplay/answer/9130646
* Turning saving off does **not** delete a copy that already exists — these are two separate actions. The App asks about deleting the copy when saving is turned off.

### 4. Purpose of Actions
The actions taken by the App are intended for:
1. **Game Functionality:** Saving game state (Save/Load) — local data and, optionally, a copy on the User's Google account.
2. **Maintenance and Development:** Monitoring crashes and statistics — only with User consent.
3. **Monetization:** Displaying ads — personalized only with User consent.
4. **Reminders:** Displaying local gameplay reminders — only with User consent and only on the device.

### 5. Data Deletion
Full control over data lies with the User.

**Managing Game Progress (Local Data):**
* **Deleting individual entries:** The User can manually delete selected results in the Statistics section.
* **Complete data deletion:** To permanently delete all progress, uninstall the app or clear its data (*Android Settings -> Apps -> Velo Sudoku -> Storage -> Clear Data*).

**Managing Copies on the Google Account:**
* **Cloud copy (Play Games):** *App Settings -> "Delete cloud copy"*. Deleting the copy does not affect the progress stored on the device. Play Games data for this game can also be deleted directly at Google: https://support.google.com/googleplay/answer/9130646
* **Android's automatic app backup:** managed in the device's system settings (*Android Settings -> Google -> Backup*) and in the User's Google Drive.

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
