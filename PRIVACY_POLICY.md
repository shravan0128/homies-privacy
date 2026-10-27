# Privacy Policy for Homies

**Effective Date:** October 26, 2026  
**Last Updated:** October 26, 2026  
**Application Name:** Homies ("the App", "we", "us", or "our")  
**Developer Contact:** support@homies.app  
**Account Deletion URL:** https://homie-514a2.web.app/delete-account  

---

## 1. Introduction

Welcome to **Homies**. We are committed to protecting your privacy and ensuring you have a secure experience when using our private calling and communication platform. This Privacy Policy describes how we collect, use, process, and safeguard your personal data when you use the Homies mobile application.

By installing or using the App, you agree to the collection and use of information in accordance with this policy.

---

## 2. Information We Collect

### A. Information You Provide to Us
- **Account Information:** When you register, we collect your email address, password (securely hashed via Firebase Authentication), chosen display name, username, and optional profile bio.
- **Profile Customization:** Selected avatar style and custom user status.
- **Messages & Shared Media:** Private chat messages, photos, videos, location coordinates, and contacts that you explicitly choose to send to your approved friends.
- **Invite Tokens:** Secure alphanumeric tokens generated when you invite friends to join your private circle.

### B. Device & Technical Information
- **Push Notification Tokens:** We collect Firebase Cloud Messaging (FCM) device tokens solely to deliver real-time incoming call alerts and chat notifications to your device.
- **Connection Data:** IP addresses and network connection parameters necessary for establishing WebRTC peer-to-peer audio and video streaming.

### C. Device Permissions & Usage
To provide real-time calling and messaging features, the App requests access to the following hardware and software capabilities:
- **Microphone (`RECORD_AUDIO`):** Required to capture your voice during 1-to-1 audio and video calls. Audio is streamed in real time via peer-to-peer WebRTC and is never recorded or stored on our servers.
- **Camera (`CAMERA`):** Required to broadcast your video during 1-to-1 video calls and to capture photos/videos for chat attachments. Video streams are peer-to-peer and never stored on our servers.
- **Location (`ACCESS_FINE_LOCATION`, `ACCESS_COARSE_LOCATION`):** Only accessed when you explicitly tap "Share Current Location" or "Start Live Location" in a private conversation. Location data is never collected in the background without your knowledge.
- **Contacts (`READ_CONTACTS`):** Only accessed when you open the "Share Contact" sheet to pick a contact to share with a friend. Your entire address book is never uploaded or harvested.
- **Photos & Videos (`READ_MEDIA_IMAGES`, `READ_MEDIA_VIDEO`):** Only accessed when you choose to attach existing media files from your device gallery.
- **Notifications (`POST_NOTIFICATIONS`):** Required on Android 13+ to alert you of incoming voice calls, video calls, and private messages.

---

## 3. How We Use Your Information

We use the collected information exclusively to:
1. Provide, maintain, and optimize 1-to-1 WebRTC audio/video calling and real-time messaging.
2. Verify member accounts and enforce our private invite-only friend circle architecture.
3. Authenticate your sign-in sessions securely.
4. Deliver high-priority incoming call alerts and chat notifications.
5. Provide accurate online/offline presence indicators to your approved friends.

---

## 4. How Your Information is Shared

**We do NOT sell, rent, monetize, or trade your personal data to any third parties or advertisers.**

Information is only processed by trusted infrastructure service providers:
- **Google Cloud / Firebase (Google LLC):** For user authentication, encrypted cloud database storage (Cloud Firestore), media storage (Firebase Storage), and push notifications (Firebase Cloud Messaging).
- **WebRTC Peer-to-Peer:** Voice and video media packets are transmitted directly between call participants using standard encrypted WebRTC protocols (DTLS/SRTP).

---

## 5. Data Retention & Complete Account Deletion

### User Deletion Rights (Google Play Policy Compliance)
You have the complete right to delete your account and all associated personal data at any time.

1. **In-App Account Deletion:**
   - Navigate to **Settings > Account > Delete Account** in the App.
   - Confirming deletion permanently and immediately erases:
     - Your Firebase Authentication credentials and sign-in record.
     - Your user profile document in Cloud Firestore (`users/{uid}`).
     - All active push notification device tokens (`fcmTokens`).
     - Your mutual friends associations, blocked users list, and call history logs.
     - Any avatar media stored in Firebase Storage.

2. **Web-Based Account Deletion Request:**
   - Users may request complete account and data deletion online without installing the app by visiting our public deletion page:  
     **https://homie-514a2.web.app/delete-account**  
   - Alternatively, email us at `support@homies.app` with the subject "Delete My Account". All data associated with the verified email will be purged within 48 hours.

---

## 6. Security & Data Protection

We implement industry-standard administrative, technical, and physical safeguards:
- All network communications between the App and Firebase/cloud servers use Transport Layer Security (TLS/HTTPS).
- WebRTC voice and video streams are end-to-end encrypted using Datagram Transport Layer Security (DTLS) and Secure Real-time Transport Protocol (SRTP).
- Database operations are constrained by strict server-side Firestore Security Rules preventing unauthorized access by unapproved users or third parties. Private conversations and messages can only be read by verified conversation participants.

---

## 7. Children's Privacy

Homies is not directed to children under the age of 13 (or 16 in certain jurisdictions). We do not knowingly collect personal identifiable information from children. If you become aware that a child has provided us with personal data without parental consent, please contact us at `support@homies.app` and we will promptly take steps to remove such information.

---

## 8. Changes to This Privacy Policy

We may update our Privacy Policy periodically. We will notify you of any changes by posting the new policy in the App and updating the "Last Updated" date at the top of this document.

---

## 9. Contact Us

If you have questions or concerns about this Privacy Policy, please contact us at:  
**Email:** `support@homies.app`  
**Web Support:** `https://homies-514a2.web.app`
