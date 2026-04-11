<div align="center">

<!-- Animated pulsing SOS button — works on GitHub -->
<svg width="200" height="200" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <!-- Pulse ring 1 -->
  <circle cx="100" cy="100" r="60" fill="none" stroke="#E24B4A" stroke-width="2">
    <animate attributeName="r" values="60;90;60" dur="2.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.8;0;0.8" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <!-- Pulse ring 2 (offset) -->
  <circle cx="100" cy="100" r="60" fill="none" stroke="#E24B4A" stroke-width="1.5">
    <animate attributeName="r" values="60;80;60" dur="2.5s" begin="0.6s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;0;0.5" dur="2.5s" begin="0.6s" repeatCount="indefinite"/>
  </circle>
  <!-- Main red circle -->
  <circle cx="100" cy="100" r="58" fill="#E24B4A"/>
  <!-- SOS text -->
  <text x="100" y="112" text-anchor="middle" font-family="Arial, sans-serif" font-size="28" font-weight="bold" fill="white" letter-spacing="4">SOS</text>
</svg>

<!-- Animated title -->
<svg width="500" height="60" viewBox="0 0 500 60" xmlns="http://www.w3.org/2000/svg">
  <text x="250" y="44" text-anchor="middle" font-family="Arial, sans-serif" font-size="36" font-weight="bold" fill="#E24B4A">
    SOS Bharat
    <animate attributeName="opacity" values="0;1" dur="1s" fill="freeze"/>
  </text>
</svg>

<!-- Animated subtitle -->
<svg width="520" height="36" viewBox="0 0 520 36" xmlns="http://www.w3.org/2000/svg">
  <text x="260" y="24" text-anchor="middle" font-family="Arial, sans-serif" font-size="15" fill="#888888">
    🚨 Emergency Alert App · Built for Every Indian Citizen 🇮🇳
    <animate attributeName="opacity" values="0;1" dur="1.5s" begin="0.5s" fill="freeze"/>
  </text>
</svg>

<!-- Live alert bar animation -->
<svg width="560" height="44" viewBox="0 0 560 44" xmlns="http://www.w3.org/2000/svg">
  <rect x="0" y="0" width="560" height="44" rx="8" fill="#3a1a1a"/>
  <!-- Blinking red dot -->
  <circle cx="22" cy="22" r="6" fill="#E24B4A">
    <animate attributeName="opacity" values="1;0.2;1" dur="1.4s" repeatCount="indefinite"/>
  </circle>
  <text x="38" y="27" font-family="Arial, sans-serif" font-size="13" fill="#cccccc">Sending SOS to contacts — GPS attached · 112 on standby</text>
</svg>

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
├── assets/images/              # App icons and images
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
3. **Auto-alert** — GPS is fetched and SMS sent to all contacts instantly.
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
