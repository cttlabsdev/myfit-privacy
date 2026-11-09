# PRIVACY POLICY FOR MY FIT AI
**Effective Date:** November 09, 2026  
**Last Updated:** November 09, 2026  
**Application ID:** `vn.cttlabs.myfit`  
**Developer:** CTT Labs  
**Contact Email:** [ctt.labs@gmail.com](mailto:ctt.labs@gmail.com)  

---

## 1. Introduction

Welcome to **My Fit AI** ("the Application", "we", "us", or "our"), developed and operated by **CTT Labs**. We respect your privacy and are committed to protecting the personal data of our users ("you" or "user").

This Privacy Policy explains how our mobile application collects, uses, stores, and protects your information in strict compliance with the **Google Play Developer Program Policies**, **General Data Protection Regulation (GDPR)**, and the **California Consumer Privacy Act (CCPA)**.

By installing, accessing, or using My Fit AI, you agree to the collection and use of information in accordance with this policy.

---

## 2. Information We Collect

### A. Information You Provide
- **Authentication Credentials:** When you choose to sign in via Google Sign-In, we receive your name, email address, and profile photo provided by Google Authentication services.
- **Physical & Fitness Metrics:** Height, body weight, target fitness goals, estimated body fat percentage, and body part measurements.
- **Workout Logs:** Exercise names, sets, repetitions, weight loads (1RM), rest timer durations, and workout notes.
- **Nutrition & Dietary Logs:** Food names, calorie intakes, macronutrients (protein, carbs, fat), and hydration logs.

### B. Device & Hardware Permissions
- **Camera (`android.permission.CAMERA`):** Used solely to take progress posture photos and capture food images for personal tracking. **All photos remain strictly stored in your device's private sandboxed local storage** and are never transmitted to external cloud servers.
- **Notifications (`android.permission.POST_NOTIFICATIONS`):** Used on Android 13+ to deliver rest interval countdowns during workouts and scheduled workout reminders.
- **Foreground Service (`FOREGROUND_SERVICE_SPECIAL_USE` & `FOREGROUND_SERVICE_MEDIA_PLAYBACK`):** Used to maintain the rest timer countdown on your lock screen and play workout music via Jetpack Media3.
- **Vibration (`android.permission.VIBRATE`):** Used to provide tactile haptic feedback when a set is completed or a rest interval expires.

### C. Automatically Collected Information
- **Diagnostic & Performance Data:** Crash logs, app performance metrics, and operating system version collected anonymously via Google Play Services to improve app stability.

---

## 3. How We Store and Protect Your Data

- **Local-First Architecture:** By default, your workout history, measurement records, and nutrition data are stored in a secure, local SQLite database on your device (Room Database).
- **No Unauthorized Sharing:** We do not sell, rent, or trade your personal information to data brokers or third parties for marketing purposes.
- **Encrypted Transmission:** All network communication (such as sign-in, Cloudflare AI proxy coaching, and AdMob requests) occurs strictly over secure, encrypted HTTPS/TLS protocols (`android:usesCleartextTraffic="false"`).

---

## 4. Third-Party Services

My Fit AI integrates reputable third-party SDKs that may collect information used to identify you in accordance with their respective privacy policies:

1. **Google Play Services & Google Identity:** For secure authentication and device integrity.  
   [Google Privacy Policy](https://policies.google.com/privacy)
2. **Google Mobile Ads (AdMob):** For serving in-app banner and rewarded ads. AdMob may collect pseudonymous advertising IDs and device identifiers.  
   [Google AdMob Privacy Policy](https://support.google.com/admob/answer/6128543)
3. **Cloudflare AI Workers Proxy:** For processing natural language AI coaching queries. Queries are processed statelessly without storing user identities.  
   [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/)

---

## 5. Account and Data Deletion Policy (Google Play Compliant)

We respect your right to access, export, and delete your personal data:

1. **In-App Immediate Deletion:**
   - Open **My Fit AI** > Navigate to **Cài đặt & Sao lưu (Settings & Backup)**.
   - Tap **"Xóa toàn bộ dữ liệu & Đăng xuất" (Delete All Data & Logout)**.
   - All local databases, cached images, and user profile records will be permanently wiped from your device.

2. **Web / Email Deletion Request:**
   - If you have uninstalled the app or wish to request full deletion of any cloud-associated records (such as Google Authentication tokens or Firebase records), email us at **[ctt.labs@gmail.com](mailto:ctt.labs@gmail.com)** with the subject `"Request Account and Data Deletion - My Fit"`.
   - Your request will be fulfilled within **48 business hours**, and a confirmation email will be sent to you.

---

## 6. Children's Privacy (COPPA)

My Fit AI is intended for general audiences aged 13 and older. We do not knowingly collect or solicit personal identifiable information from children under 13. If you believe that a child under 13 has provided us with personal data, please contact us immediately, and we will promptly delete such information.

---

## 7. Changes to This Privacy Policy

We may update our Privacy Policy periodically to reflect app enhancements or legal requirements. Any modifications will be posted on this page with an updated "Last Updated" date.

---

## 8. Contact Us

If you have questions, feedback, or data privacy requests regarding this Privacy Policy, please contact:

- **Developer:** CTT Labs  
- **Package Name:** `vn.cttlabs.myfit`  
- **Email:** [ctt.labs@gmail.com](mailto:ctt.labs@gmail.com)  
- **Website:** [https://cttlabs.github.io/myfit](https://cttlabs.github.io/myfit)
