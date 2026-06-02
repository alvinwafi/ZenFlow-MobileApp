
# 🌊 ZenFlow — Mobile

**ZenFlow Mobile** is the Android companion to [ZenFlow](https://github.com/placeholder/zenflow), bringing the same calm, focused productivity experience to your phone. Built with Expo and React Native, it features a touch-optimized UI, push notifications, and full Supabase cloud sync — so your tasks, habits, and sessions stay in perfect harmony across devices.

> 🔒 **This is a closed-source project.** Only the APK is distributed publicly. The source code is not available.

---

## 🎯 Purpose

ZenFlow Mobile was built to extend the ZenFlow desktop experience to Android — giving students, freelancers, and remote workers the same distraction-free, habit-building workspace in their pocket. Whether you're away from your desk or on the move, your focus sessions, task list, and habit streaks are always with you.

---

## 🧠 Features

- ⏳ **Pomodoro Timer** — Time-blocked work sessions with auto-logging, sound alerts, customizable durations, and autostart support.
- ✅ **Task Checklist** — Add, complete, archive, and manage daily to-dos with a completed tasks history.
- 📅 **Habit Log (Heatmap)** — Visualize your daily consistency with a full-year calendar heatmap.
- 🧮 **Calculator** — A minimal, keyboard-friendly calculator built right into your workspace.
- 📊 **Stats Dashboard** — Track your Pomodoro sessions, focus time, and productivity trends over time.
- 👤 **Profile & Avatar** — Personalize your experience with a display name, emoji avatar, and custom status.
- ☁️ **Cloud Sync (Supabase)** — Sign up or log in to sync your tasks, habits, sessions, and profile across devices — including with the desktop app.
- 🔒 **Offline-First** — All data is stored locally and works fully without internet.
- 📲 **Touch-Optimized UI** — Every screen is redesigned for mobile interaction, with gesture-friendly layouts and native feel.

---

## 🧱 Tech Stack

ZenFlow Mobile is a React Native application built with Expo, featuring local persistence and optional Supabase cloud sync.

### 📱 Front-End
- **Expo** — Managed React Native workflow for cross-platform development
- **React Native** — Core mobile UI framework
- **React Navigation** — Screen routing and navigation stack
- 
### 🧠 Back-End & Data
- **Supabase JS SDK** — Cloud authentication and real-time database sync
- **AsyncStorage** — Local offline-first data persistence
- **Expo SecureStore** — Secure storage for auth tokens and credentials
- **dotenv / app.config.js** — Environment variable management for Supabase credentials

---

## 🛠 Built With

| Package | Purpose |
|---|---|
| `expo` ~51 | Managed React Native workflow |
| `react-native` 0.74 | Mobile UI framework |
| `@react-navigation/native` ^6 | Screen navigation |
| `@supabase/supabase-js` ^2.49 | Cloud auth and data sync |
| `@react-native-async-storage/async-storage` | Local offline persistence |
| `expo-notifications` | Push notification support |
| `react-native-reanimated` ^3 | Animations and transitions |
| `expo-secure-store` | Secure token storage |
| `expo-av` | Audio playback for timer alerts |

---

## 📲 Installation

ZenFlow Mobile is distributed as an Android APK. No Play Store listing — just download and install directly.

### 🔧 Requirements

- Android 10 (API 29) or higher
- ~100 MB free storage
- Internet connection (optional — only needed for cloud sync)

### 📦 Download & Install

1. **Download the latest APK** from the [Releases](https://github.com/alvinwafi/ZenFlow-MobileApp/releases/download/apk/ZenFlow.apk) page.

2. **Enable installation from unknown sources** on your Android device:
   - Go to **Settings → Security** (or **Settings → Apps → Special app access**)
   - Enable **Install unknown apps** for your browser or file manager

3. **Open the downloaded APK** and tap **Install**.

4. **Launch ZenFlow** from your app drawer and enjoy. ✨

> **Note:** You may see a Google Play Protect warning since the APK is not distributed through the Play Store. Tap **Install anyway** to proceed.

---

## ☁️ Cloud Sync

ZenFlow Mobile shares the same Supabase backend as the desktop app. Sign in with the same account to sync your data seamlessly across both platforms.

Your data syncs automatically on login. All tables use Row Level Security (RLS) — your data is only ever accessible to you.

| Table | Key Columns |
|---|---|
| `profiles` | `id`, `display_name`, `avatar_emoji`, `status`, `theme`, `pref_*`, `focus_log` |
| `habit_days` | `user_id`, `day`, `level` |
| `tasks` | `user_id`, `title` |
| `tasks_completed` | `user_id`, `title`, `completed_at` |
| `pomodoro_sessions` | `user_id`, `session_date`, `completed_at` |

---

## 🖥️ System Requirements

| Requirement | Minimum |
|---|---|
| **OS** | Android 10 (API 29) |
| **RAM** | 3 GB |
| **Storage** | 100 MB free |
| **Display** | 360×640 resolution or higher |

---

## 🔒 Source Code

This project is **closed source**. The APK is provided as-is for personal use. The source code is not publicly available and is not open for contributions at this time.

---

## 📜 License

This project is licensed under the **MIT License**.
See the [LICENSE](./LICENSE) file for more details.

The APK is free to download and use for personal, non-commercial purposes.

---

## 🙏 Acknowledgements

ZenFlow Mobile was inspired by the same tools that shaped the desktop version:

- [Studyverse](https://studyverse.life/) (R.I.P.)
- [LifeAt](https://lifeat.io/)
- [PomoFocus](https://pomofocus.io/)

---

## 👥 Team

- [Sumerah Tasmiah Khan](https://github.com/theweirdsumerah)
- [Alvin Rahman Wafi](https://github.com/alvinwafi)

Also check out 🖥️ [ZenFlow Desktop](https://github.com/theweirdsumerah/ZenFlow-WebApp) — the Electron version this app is based on.

---

<p align="center">Built with love and focus. 🌊</p>
