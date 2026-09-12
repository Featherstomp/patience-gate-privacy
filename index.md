# Patience Gate — Privacy Policy

**Last updated:** 12 September 2026

**Developer:** Patience Gate
**Contact for privacy questions:** patiencegateapp@gmail.com

---

## The short version

Patience Gate does not collect your data. It does not send anything anywhere. It has no analytics, no advertising, no third-party components, and no account system.

The app does not have permission to access the internet at all. This is not a policy promise — the Android permission that would allow network access (`android.permission.INTERNET`) is not declared in the app, which means the operating system itself prevents the app from making any network connection. Anyone can verify this by inspecting the app package.

Everything below explains this in more detail.

---

## 1. Who this policy applies to

This policy covers the Patience Gate Android application published on Google Play by Patience Gate.

Patience Gate is a parental-control tool. It is intended to be installed by an adult on a phone that adult owns, and used while a young child is briefly holding that phone. It is also used by some people to limit their own short-form video use.

---

## 2. What the app accesses on your device

Patience Gate uses Android's Accessibility Service to do its one job: pausing the swipe-to-next-video gesture in the YouTube app's Shorts feed until the current video has finished playing.

To do that, while the YouTube Shorts feed is open, the app reads the following from the screen:

- **How long the current video is, and how far it has played.** Read from the on-screen progress bar's accessibility description.
- **A short identifier for the current video.** Built by taking the visible caption text and creator handle and converting them into a fixed-length code (a hash). This is used only to notice when the video on screen has changed. The original text is not kept.
- **Whether the current item is an advertisement.** Detected from the on-screen "Ad" or "Sponsored" label, so the app can stand down completely. Patience Gate never blocks, delays, skips, or interacts with advertising.
- **Whether the Shorts feed is currently on screen at all.** So the app can stop acting the moment you leave it.

All of this is read in the moment, used immediately, and discarded. None of it is written to storage. None of it is transmitted.

**The app does not read, store, or transmit:**

- The content of videos, images, or audio
- Which specific videos were watched, or a history of them
- Anything from other apps — the accessibility service is scoped to the YouTube app
- Messages, emails, contacts, photos, files, or browsing history
- Passwords, payment details, or anything typed into any field
- Location
- Any device identifier, advertising ID, or account identifier

---

## 3. What the app stores on your device

A small amount of information is saved on the phone itself, in the app's private storage. It never leaves the device.

- **Your settings.** Whether the gate is switched on, and whether optional features are enabled.
- **Technical fault records.** If the app loses track of what YouTube is showing, it stops blocking (it fails open, so a child is never trapped on a video) and records that this happened. Each record contains only: a fixed internal name for which part of the app had trouble, a timestamp, the app version, and the Android version. It contains nothing about what was being watched, nothing about the user, and no identifiers of any kind.

The app's screen includes a "Send this report" option for these fault records. **In the current version this does not transmit anything.** Because the app has no internet permission, it cannot. The option writes the report to the phone's local system log only. If a future version of the app ever transmits these reports, this policy will be updated before that version is released, and it will remain something you actively choose each time — never automatic.

---

## 4. Data retention and deletion

Because no data leaves your device, there is nothing held by the developer to retain or delete. There is no server, no database, and no copy of anything from your phone.

Everything the app stores is held in Android's standard app-private storage. You can remove all of it at any time by:

- Going to **Settings → Apps → Patience Gate → Storage → Clear data**, or
- Uninstalling the app, which deletes all of it automatically.

No request to the developer is needed, and there is nothing for the developer to delete on your behalf.

---

## 5. Accessibility Service disclosure

Patience Gate requests permission to use Android's Accessibility Service. Android shows you a warning when you enable this, and the app shows you its own explanation screen beforehand, which you must acknowledge before continuing.

Patience Gate is declared to Google Play as a **monitoring tool** (`isMonitoringTool`), not as an accessibility tool. It is a parental-control app, not a tool for users with disabilities, and it does not claim otherwise. Because of this declaration, Google Play Protect may show a notice on the device stating that a monitoring application is installed. This is intentional and correct.

The accessibility permission is used solely for the purpose described in section 2. It is not used to log activity, build a profile, monitor behaviour over time, or observe anything outside the YouTube Shorts feed.

You can turn the accessibility permission off at any time in **Settings → Accessibility**, and the app stops doing anything immediately.

---

## 6. Children's privacy

Patience Gate is designed to be used while a young child holds an adult's phone. It is installed and controlled by an adult.

The app collects no personal information from anyone, including children. It does not build profiles, does not track behaviour across sessions, does not store any history of what was watched, and transmits nothing off the device. There is no mechanism by which information about a child using the phone could reach the developer or any third party.

---

## 7. Third parties

Patience Gate contains no third-party software development kits, no analytics libraries, no crash-reporting services, and no advertising components. No third party receives any information from this app.

Patience Gate interacts with the YouTube app only by reading what is on screen, as described above. It does not connect to YouTube's servers, does not have a YouTube account, and does not modify YouTube in any way. Your use of YouTube is governed by Google's own terms and privacy policy, not this one.

---

## 8. Security

Because nothing is transmitted, there is no data in transit to intercept and no server to breach. Information stored on the device is held in Android's app-private storage, which the operating system protects from other apps.

---

## 9. Changes to this policy

If this policy changes, the updated version will be posted at this address and the "last updated" date above will change. If a future version of the app ever transmits any information off the device, this policy will be updated to say so clearly **before** that version is released.

---

## 10. Contact

Questions about this policy, or about privacy in Patience Gate:

**patiencegateapp@gmail.com**
