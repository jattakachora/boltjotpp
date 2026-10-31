# BoltJot Privacy Policy

**Effective date:** 31 October 2026
**App:** BoltJot (package `com.apphux.boltjot`), published under the apphux brand
**Developer and data controller:** Rajneesh Kumar, United Kingdom
**Contact:** apphux@gmail.com

BoltJot is a note-taking app that keeps your notes on your device. This policy explains what the app handles, what leaves your device, and the choices you have. BoltJot has no user accounts, no ads, no analytics service and no developer-run server.

## 1. Summary

- Your notes, labels, reminders, attachments and settings are stored on your device.
- We do not receive your notes. We do not sell your data or use it for advertising.
- Data leaves your device only when you use an optional feature (Google Drive backup, a local backup you export, PC Dashboard, a YouTube link preview), or through the services listed in section 6 (crash reports, Google Play purchases, and Google's own device backup).
- BoltJot is for people aged 13 and over.

## 2. Data the app handles

| Data | Purpose | Where it is kept |
|---|---|---|
| Notes: titles, text, checklists, labels and sub-labels, pins, colours, trash | The app's core function | On your device |
| Reminders and schedules | To notify you at the time you choose | On your device |
| Photos, videos, scanned documents, drawings | Attaching media to notes | On your device |
| Audio recordings | Voice notes | On your device |
| Location (optional): coordinates, accuracy and a map link | Stamping a note with where you were, only if you enable automatic location or attach it | On your device, in the note |
| Text recognised from scanned documents | Making scanned pages searchable | On your device (processed on-device) |
| Settings, widget appearance, backup schedule | Remembering your choices | On your device |
| Label PIN and PC Dashboard password | Restricting access inside the app | On your device, as salted hashes protected by an Android Keystore key |
| Pro purchase status | Unlocking paid features | On your device, encrypted with an Android Keystore key; purchase processing is by Google Play |
| Google account ID and email (only if you sign in for Drive backup) | Backing up to your own Drive and restoring | On your device; sent to Google as part of sign-in |
| Crash reports (see section 6.3) | Finding and fixing crashes | Sent to Google (Firebase Crashlytics) |

Your notes, media and audio are not encrypted by BoltJot on the device itself. They are protected by Android's app sandbox and your device's own encryption and screen lock. The label PIN restricts access inside the app. It does not encrypt your content.

## 3. Permissions explained

| Permission | What it is for |
|---|---|
| Camera | Taking photos, videos and document scans for notes. Asked when you use it. |
| Microphone | Recording voice notes. Asked when you use it. |
| Location (precise and approximate) | The optional location stamp on notes. Asked only if you turn on automatic location or attach a location. |
| Notifications | Reminders, the lock-screen quick-capture notification, pinned notes, and the PC Dashboard indicator. |
| Exact alarms | Delivering note reminders at the exact time. If it is off, reminders still work but may arrive late. |
| Run at start-up | Restoring reminders and the quick-capture notification after your phone restarts. |
| Foreground service | Keeping the quick-capture notification and the PC Dashboard server running. |
| Biometric / screen lock | Confirming it is you before opening protected settings and recovery. |
| Internet and network state | Google Drive backup, crash reports, Google Play, YouTube link previews, and checking that you are on Wi-Fi when a backup is set to Wi-Fi only. |
| Photos, files and folders | BoltJot does not request broad access to your photos or files. It only reads the photos, files or folders you choose through Android's picker, or share into the app. |

You can turn permissions off in Android Settings. The features that depend on them will stop working, and your existing notes are unaffected.

## 4. Lock-screen quick capture

BoltJot can show a persistent notification and a Quick Settings tile that open a capture screen above your lock screen. There is no screen overlay. Please note:

- Anyone holding your locked phone can use the capture screen to add a new note (including a photo, audio or location). It does not show your existing notes, and labels you have protected are hidden while the phone is locked.
- Notes you pin to the lock screen appear in a notification showing the title and the first 100 characters of the note. Whether that is visible on the lock screen depends on your Android settings. Notes you mark private are not shown.

## 5. Optional features that move data

### 5.1 Google Drive backup (optional)

If you sign in with Google, BoltJot can upload a backup to a folder named "BoltJot Backups" in your own Google Drive, manually or on a schedule. It asks only for the `drive.file` permission, which lets BoltJot see only the files it created. BoltJot also reads your Google account ID and email address to identify the account.

- **What is in a backup:** notes, labels, attachments, audio, drawings, scans, and any note locations. Reminders are not included. It is packaged and encrypted on your device with AES-256-GCM before upload.
- **How strong the encryption is:** the encryption key is derived from your Google account ID, so you can restore on a new phone by signing in with the same account and no password. This protects the file from casual viewing, but it is not end-to-end encryption and it is not a secret that only you hold. Do not treat a Drive backup as protection against someone who has access to your Google account.
- **What is not encrypted:** the file name, size and date, and the folder name, which Google can see.
- **Retention:** BoltJot keeps your five newest backups and deletes older ones.
- Transfers use HTTPS and, by default, Wi-Fi only.
- We do not receive your backups. They are stored in your Drive.

Google API data is used only to provide this backup and restore feature. It is not sold, not used for advertising, and not transferred to third parties except as needed to provide the feature, and BoltJot's use of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including its Limited Use requirements.

### 5.2 Local backup (optional)

You can export a backup file to a folder you choose, manually or on a schedule. It is encrypted with AES-256-GCM using a password you set and a random salt. We cannot recover the password or the file. You are responsible for the file's location and for keeping the password safe.

### 5.3 PC Dashboard (optional, Pro)

PC Dashboard runs a small web server on your phone so you can use your notes from a computer's browser on the same private Wi-Fi network. It does not send your notes to us or to any cloud service.

- It uses unencrypted HTTP. Anyone on the same network could potentially see traffic while a session is open. Use it only on a trusted private network.
- A computer must be approved on your phone with a short code. Sessions expire after inactivity.
- It requires a screen lock on your phone and an acknowledgement of this warning.

### 5.4 Link previews

If you paste a YouTube link into a note, BoltJot can show an embedded player from `youtube-nocookie.com`. This contacts Google/YouTube and sends technical data such as your IP address and the video requested. Other links are not fetched. They open in your browser only when you tap them.

## 6. Third-party services

BoltJot uses these services. Each is governed by its own policy.

1. **Google Drive and Google Sign-In** (section 5.1). [Google Privacy Policy](https://policies.google.com/privacy).
2. **Google Play Billing.** Purchases of BoltJot Pro are handled by Google Play. We do not receive your payment details. BoltJot keeps an encrypted record of purchase status on your device.
3. **Firebase Crashlytics (Google).** When the app crashes, a report is sent to Google containing the technical stack trace (class names and code locations only, not exception messages or your note content), app version, Android version, device model, a few fixed labels such as the screen you were on, and a Firebase installation identifier. Google also receives your IP address as part of the connection. We use this only to find and fix bugs. Crash reporting is always on. See [Firebase privacy information](https://firebase.google.com/support/privacy).
4. **Google ML Kit.** Text recognition and the document scanner run on your device. Google may collect technical usage and performance metrics from these SDKs, as described in [ML Kit's data disclosure](https://developers.google.com/ml-kit/android-data-disclosure).
5. **YouTube** (section 5.4). [YouTube Terms and Google Privacy Policy](https://policies.google.com/privacy).
6. **Android's backup service (Google).** Android's own backup, if you have it turned on in your phone settings, may include BoltJot's notes, media and settings in your Google backup and when transferring to a new phone. That is controlled by Google and your device settings, not by BoltJot. BoltJot excludes your label PIN and dashboard credentials from this backup.

We do not sell your data, share it for advertising, or give it to data brokers. We do not use advertising or analytics SDKs.

## 7. Security

- Local-first storage, with no developer server holding your notes.
- Backups are encrypted before leaving your device (with the limits described in section 5.1).
- Label PIN and dashboard password are stored as salted hashes protected by a hardware-backed Keystore key where your device supports it, with lockout after repeated failures.
- Crash reports exclude exception messages and note content.
- No system is perfectly secure. Keep your phone locked, and keep your device and apps updated.

## 8. Retention and deletion

- **On your device:** data stays until you delete it. Deleted notes go to Trash until you empty it or delete them permanently. Uninstalling BoltJot or clearing its storage removes everything stored by the app on the device.
- **Google Drive backups:** in BoltJot's backup settings, delete any listed backup. Signing out of Google in BoltJot does not delete your backups, and neither does uninstalling the app. You can also delete the "BoltJot Backups" folder in Google Drive, and remove BoltJot's access at myaccount.google.com/permissions (this does not delete the files).
- **Local backups and exports:** these stay where you saved them until you delete them there.
- **Android device backup:** manage or delete it in your Google/Android backup settings.
- **Crash reports:** these are held by Google under Firebase's retention rules. We cannot link a report to you personally, so we cannot look up reports by name or email.
- **Support emails:** kept for as long as reasonably needed to deal with your request.

## 9. Your rights

Depending on where you live (including under UK GDPR), you may have the right to access, correct, delete, restrict or object to the use of your personal data, and to data portability. Because your notes are on your device, you can exercise most of these yourself in the app (including by exporting or deleting your notes). For anything else, email apphux@gmail.com. UK users can also complain to the Information Commissioner's Office (ico.org.uk).

If you email support from within the app, the email may include your app version, Android version and device model that you can review and edit before sending.

## 10. Children

BoltJot is a general productivity app for people aged 13 and over. It is not directed to children under 13, and we do not knowingly collect personal information from them. If you believe a child under 13 has used the app, contact apphux@gmail.com.

## 11. International transfers

Google services (Drive, Crashlytics, Google Play, YouTube) may process data in countries outside your own, under Google's own safeguards.

## 12. Changes to this policy

If we change this policy, we will update the date at the top and, for significant changes, tell you in the app or on the app's store listing. Continued use after a change means you accept it.

## 13. Contact

Rajneesh Kumar (apphux), United Kingdom
Email: apphux@gmail.com
