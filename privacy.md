# EchoLink — Privacy Policy

**Last updated:** 2026-05-02
**Effective date:** 2026-05-02

This Privacy Policy explains how EchoLink ("we", "us", "the app") collects, uses, and shares personal data when you use the EchoLink mobile application.

We comply with the EU General Data Protection Regulation (Regulation (EU) 2016/679, "GDPR") and the Italian Personal Data Protection Code (D.Lgs. 196/2003 as amended by D.Lgs. 101/2018).

---

## 1. Data we collect

### 1.1 Account data
When you create an account we collect:
- **Email address** and **password** (password is hashed by our authentication provider — we never see it in plain text)
- **Display name** (chosen by you)
- **Profile picture** (optional, uploaded by you)

You may also use the app **anonymously** without creating an account. In anonymous mode we generate a random identifier (UUID) stored locally on your device. No email is required.

### 1.2 Music listening data ("now-playing")
When music scrobbling is enabled, we collect the **track name, artist, album, album artwork URL, source app name, and play/pause state** of the music playing on your device. This data is shared with users who follow you.

We collect this data through:
- The **Spotify SDK**, if you have linked your Spotify account
- The **Android notification listener**, which reads notifications **only from music apps** (Spotify, YouTube Music, Apple Music, Tidal, Deezer, SoundCloud, Amazon Music, Pandora, TuneIn, and apps whose package name contains "music", "radio", "audio", or "player"). Non-music notifications are silently discarded and never stored or transmitted.
- **Last.fm**, if you have linked your Last.fm account

You can disable scrobbling at any time in **Settings → Scrobbling**.

### 1.3 Location data
If you enable **Nearby Discovery**, we collect your **approximate GPS coordinates (latitude, longitude)** to show you to nearby users. Location is collected via the Android Fused Location Provider and is updated approximately every 30 seconds while the feature is enabled.

You can:
- Disable Nearby Discovery entirely in Settings
- Toggle **Ghost Mode** to immediately remove your location from our servers without disabling the feature

We do **not** collect precise location history, only your most recent position. Each position overwrites the previous one.

### 1.4 Bluetooth (BLE) peer-to-peer data
EchoLink can advertise your currently-playing track over Bluetooth Low Energy to nearby phones, and scan for similar advertisements from other users. The advertised packet contains: song name, artist name, play/pause state, and a hashed pseudonym derived from your username.

**This data never leaves your device** — it is exchanged only directly between phones via Bluetooth radio. We do not receive, log, or store BLE data on our servers.

### 1.5 Social graph data
- **Follow / unfollow relationships**
- **Direct messages** (1-to-1 and group), including text content, reactions, read receipts, and any optional shared track data
- **Blocked users**

### 1.6 Push notification token
When you grant notification permission, your device's **Firebase Cloud Messaging (FCM) token** is stored so we can deliver push notifications (e.g., new messages). The token contains no personally identifying data on its own.

### 1.7 Linked third-party service identifiers
If you optionally connect Spotify or Last.fm, we store:
- Your Spotify user ID
- Your Last.fm username

These are used solely to attribute scrobbles correctly and can be disconnected at any time in Settings.

### 1.8 Data we do NOT collect
- We do **not** use analytics SDKs (no Google Analytics, Firebase Analytics, Mixpanel, PostHog, Sentry, etc.)
- We do **not** use crash reporting or telemetry
- We do **not** track advertising identifiers (no IDFA, no AAID)
- We do **not** read non-music notifications
- We do **not** use cookies (the app contains no embedded web tracking)

---

## 2. Legal bases for processing (GDPR Article 6)

| Data | Legal basis |
|---|---|
| Account email, password, display name | **Contract** (Art. 6(1)(b)) — necessary to provide the service you signed up for |
| Now-playing data | **Consent** (Art. 6(1)(a)) — collected only when scrobbling is enabled |
| Location | **Consent** (Art. 6(1)(a)) — collected only when Nearby Discovery is enabled |
| BLE broadcasts | **Consent** (Art. 6(1)(a)) — collected only when nearby discovery scanning is active |
| Direct messages | **Contract** (Art. 6(1)(b)) — necessary for messaging functionality |
| FCM token | **Legitimate interest** (Art. 6(1)(f)) — to deliver notifications you've opted into |
| Linked Spotify/Last.fm IDs | **Consent** (Art. 6(1)(a)) — collected only if you connect those services |

You can withdraw consent at any time by toggling the relevant feature off in Settings or by deleting your account.

---

## 3. Who we share data with

EchoLink uses the following processors. We do not sell or rent your data to anyone.

| Processor | Purpose | Location | Safeguards |
|---|---|---|---|
| **Supabase, Inc.** | Database, authentication, file storage | USA / EU | EU Standard Contractual Clauses |
| **Google LLC (Firebase Cloud Messaging)** | Push notification delivery | USA | EU Standard Contractual Clauses |
| **Spotify AB** (if you connect Spotify) | Read currently-playing track | EU / USA | Direct connection from your device — we do not proxy this data |
| **Last.fm Ltd.** (if you connect Last.fm) | Scrobble attribution | UK / EU | Direct connection from your device |
| **Apple App Store / Google Play** | App distribution | USA | Their respective privacy policies apply during installation |

**International transfers:** Some processors are based outside the EU/EEA. Where this is the case, we rely on the European Commission's **Standard Contractual Clauses (SCCs)** as the lawful transfer mechanism under Articles 45–49 GDPR.

We share follower/follow data, profile data, and now-playing/location data **with other EchoLink users** in accordance with your privacy settings (e.g., who follows you, whether Ghost Mode is on).

---

## 4. Data retention

| Data | Retention period |
|---|---|
| Account data | Until you delete your account, then deleted within 30 days |
| Now-playing | Indefinitely while account is active; overwritten on each new track |
| Location | Most recent position only (overwritten); deleted on Ghost Mode or feature disable |
| Messages | Indefinitely while either participant has an active account |
| Anonymous-mode data | Stored locally on device only; deleted on app uninstall |
| FCM token | Until permission revoked or account deleted |
| Server logs | 30 days |

---

## 5. Your rights under GDPR

You have the right to:

- **Access** the personal data we hold about you (Art. 15)
- **Rectify** inaccurate data (Art. 16)
- **Erasure / "right to be forgotten"** (Art. 17) — see Section 6
- **Restrict processing** (Art. 18)
- **Data portability** — receive your data in a machine-readable format (Art. 20)
- **Object to processing** (Art. 21)
- **Withdraw consent** at any time (Art. 7(3))
- **Lodge a complaint** with your data protection authority. In Italy: **Garante per la protezione dei dati personali** ([www.garanteprivacy.it](https://www.garanteprivacy.it))

To exercise any right, email us at **{contact@echolink.app}**. We respond within 30 days.

---

## 6. Account deletion

You can delete your account at any time from **Settings → General → Account → Delete Account**. The deletion is immediate and permanent.

When you delete your account we erase:
- Your user record (email, display name, avatar)
- Your authentication credentials
- Your now-playing entries
- Your location entry
- Your FCM push token
- Your linked Spotify/Last.fm identifiers
- Your friendships (follows in both directions)
- Your blocked-users list
- Your conversation participation
- Your message-request history

**Messages you have sent** are retained in the recipient's inbox with the sender field anonymized — the recipient retains the conversation as their own data, but the messages no longer link back to you. The recipient may delete them independently.

If self-service deletion fails for any reason, email **{contact@echolink.app}** and we will erase your data manually within 30 days.

---

## 7. Children

EchoLink is **not intended for children under 16**. We do not knowingly collect personal data from anyone under 16. If you are a parent or guardian and believe your child has provided us with personal data, contact us and we will delete it.

In countries where the age of digital consent under GDPR Art. 8 is lower than 16, the local minimum applies. In Italy the minimum is **14**.

---

## 8. Security

- All data in transit is encrypted with TLS 1.2+
- Passwords are hashed by Supabase Auth using bcrypt
- Local secrets on your device are stored using the OS-provided secure storage (Android Keystore / iOS Keychain via expo-secure-store)
- Access to backend data is restricted by Supabase Row-Level Security policies

No system is perfectly secure. If we become aware of a breach affecting your data, we will notify you without undue delay and within 72 hours as required by Art. 33–34 GDPR.

---

## 9. Changes to this policy

We may update this policy as the app evolves. Material changes will be announced in-app and by updating the "Last updated" date at the top. Continued use of the app after a change constitutes acceptance.

---

## 10. Contact

- **Email:** {app.echolink@gmail.com}
