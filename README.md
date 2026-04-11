<div align="center">

<img src="assets/sos_pulse.svg" width="160" alt="SOS Bharat Logo"/>

<img src="assets/title.svg" width="400" alt="SOS Bharat"/>

**Emergency Alert App for Every Indian Citizen**

<img src="assets/live_alert.svg" width="500" alt="Live Alert Status"/>

<br/>

[![React Native](https://img.shields.io/badge/React_Native-Expo-black?style=flat-square&logo=expo)](https://expo.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-84.9%25-3178C6?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20iOS-brightgreen?style=flat-square)](https://reactnative.dev/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-orange?style=flat-square)](https://github.com/khushijohari14/sos-bharat-app/pulls)

</div>

---

## 📖 About

SOS Bharat is a front-end emergency alert mobile app built for India. In a critical moment — a medical emergency, a fire, a security threat — you shouldn't be fumbling with your phone. **One tap** sends your live GPS coordinates via SMS to every contact you trust. No internet. No delay.

> Built for Police 🚔 · Fire 🔥 · Medical 🏥 · Women Safety 👩 — and more.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| ⚡ **One-Tap SOS** | Sends an emergency alert instantly with a single tap |
| 📍 **Live GPS Location** | Attaches real-time coordinates to every alert |
| 💬 **SMS-Based Alerts** | Works without internet — pure SMS delivery |
| 👥 **Emergency Contacts** | Add and manage your trusted contacts |
| 📞 **Direct 112 Calling** | One-tap call to India's national emergency number |
| 🗂️ **Emergency Categories** | Police · Fire · Medical · Women Safety & more |
| 🔐 **OTP Login** | Secure phone-number based authentication |
| 🗺️ **State Selector** | Localized experience based on your state |
| ✨ **Smooth Animations** | Polished UI with fluid transitions |

---

## 🛠️ Tech Stack

```
React Native (Expo)    →  Cross-platform mobile framework
TypeScript / ES6       →  Primary language (84.9% of codebase)
expo-location          →  Live GPS coordinates
expo-sms               →  SMS alert delivery
React Navigation       →  Screen routing
AsyncStorage           →  Local contact persistence
```

---

## 📁 Project Structure

```
sos-bharat-app/
├── app/                        # Screens & routing (Expo Router)
├── components/                 # Reusable UI components
├── constants/                  # Colors, strings, config
├── hooks/                      # Custom React hooks
├── sos-bharat/                 # Core SOS feature logic
├── assets/                     # App icons, images & animated SVGs
├── scripts/                    # Utility scripts
├── EmergencyAlertScreen.js     # SOS alert trigger screen
├── EmergencyContactsScreen.js  # Emergency contacts manager
├── app.js                      # App entry point
└── app.json                    # Expo configuration
```

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) v18+
- [Expo CLI](https://docs.expo.dev/get-started/installation/)
- Expo Go app on your Android/iOS device

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/khushijohari14/sos-bharat-app.git

# 2. Navigate into the project
cd sos-bharat-app

# 3. Install dependencies
npm install

# 4. Start the Expo server
npx expo start
```

> Scan the QR code with **Expo Go** to run instantly on your phone.

---

## 📲 How It Works

```
[User] ──tap──▶ [SOS Button]
                    │
                    ▼
           [Fetch live GPS via expo-location]
                    │
                    ▼
           [Compose SMS with coordinates]
                    │
                    ▼
   [Send to all saved contacts via expo-sms]
                    │
                    ├──▶ Contact 1 ✅
                    ├──▶ Contact 2 ✅
                    └──▶ Contact 3 ✅

   [Parallel] ──▶ Direct 112 dial available at all times
```

1. **Set up contacts** — Add trusted emergency contacts.
2. **In an emergency** — Tap the SOS button.
3. **Auto-alert** — GPS fetched and SMS sent to all contacts instantly.
4. **Call 112** — Dedicated button for national emergency services.

---

## 🔮 Roadmap

- [ ] Backend integration for real-time location tracking
- [ ] WhatsApp & email alert support
- [ ] Shake-to-SOS — hands-free activation
- [ ] Offline maps
- [ ] Multi-language support (Hindi + regional languages)
- [ ] Admin dashboard for NGOs / rescue organizations

---

## 🤝 Contributing

```bash
# Fork → Branch → Commit → Pull Request
git checkout -b feature/your-feature-name
git commit -m "Add: your feature description"
git push origin feature/your-feature-name
```

---

## 👩‍💻 Author

**Khushi Johari** · [GitHub](https://github.com/khushijohari14)

---

## 📄 License

Licensed under the [MIT License](LICENSE).

---

<div align="center">
  <sub>🇮🇳 Built with care for the safety of every Indian citizen.</sub>
</div>
