<div align="center">

# 🚨 SOS Bharat

### Emergency Alert App for India

**A React Native mobile app that sends instant SOS alerts with live GPS location to your trusted contacts — built for every Indian citizen.**

[![React Native](https://img.shields.io/badge/React_Native-Expo-blue?logo=expo)](https://expo.dev/)
[![Language](https://img.shields.io/badge/Language-TypeScript%20%7C%20JavaScript-yellow)](https://www.typescriptlang.org/)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20iOS-green)](https://reactnative.dev/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

</div>

---

## 📖 About

SOS Bharat is a front-end emergency alert mobile application designed to help users in India quickly reach out for help during critical situations. With a single tap, it sends an SOS message along with your **live GPS location** to your saved emergency contacts via SMS — no internet required for alerts.

Whether it's a medical emergency, a fire, a safety threat, or a situation requiring police help, SOS Bharat puts help at your fingertips.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🆘 **One-Tap SOS Alert** | Send an emergency alert instantly with a single tap |
| 📍 **Live GPS Location** | Automatically attaches your real-time coordinates to every alert |
| 📱 **SMS-Based Alerts** | Sends alerts via SMS — works without internet |
| 👥 **Emergency Contacts** | Add and manage your trusted emergency contacts |
| 📞 **Direct 112 Calling** | One-tap call to India's national emergency number |
| 🗂️ **Emergency Categories** | Quick access to Police, Fire, Medical, Women Safety & more |
| 🔐 **OTP Login** | Secure phone number-based OTP authentication |
| 🗺️ **State Selector** | Localized experience based on your state |
| 🎨 **Smooth Animations** | Polished UI with fluid transitions |

---

## 🛠️ Tech Stack

- **Framework:** React Native (Expo)
- **Language:** TypeScript / JavaScript (ES6)
- **Location:** `expo-location` — for live GPS coordinates
- **Messaging:** `expo-sms` — for sending SMS alerts
- **Navigation:** React Navigation
- **Storage:** AsyncStorage — for persisting emergency contacts locally

---

## 📁 Project Structure

```
sos-bharat-app/
├── app/                        # App screens and routing (Expo Router)
├── components/                 # Reusable UI components
├── constants/                  # App-wide constants (colors, strings, etc.)
├── hooks/                      # Custom React hooks
├── scripts/                    # Utility scripts
├── sos-bharat/                 # Core SOS feature logic
├── assets/images/              # App images and icons
├── EmergencyAlertScreen.js     # SOS alert trigger screen
├── EmergencyContactsScreen.js  # Manage emergency contacts screen
├── app.js                      # App entry point
└── app.json                    # Expo configuration
```

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or above)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)
- A physical Android/iOS device or emulator

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/khushijohari14/sos-bharat-app.git

# 2. Navigate into the project
cd sos-bharat-app

# 3. Install dependencies
npm install

# 4. Start the Expo development server
npx expo start
```

Scan the QR code with the **Expo Go** app on your phone to run it instantly.

---

## 📲 How It Works

1. **Set up contacts** — Add your trusted emergency contacts (family, friends) in the app.
2. **In an emergency** — Tap the SOS button on the home screen.
3. **Auto-alert** — The app fetches your live GPS location and sends an SMS to all saved contacts with your coordinates.
4. **Call 112** — Use the direct dial button to reach national emergency services instantly.

---

## 🔮 Roadmap / Future Scope

- [ ] Backend integration for real-time tracking
- [ ] WhatsApp/email alert support
- [ ] Shake-to-SOS trigger (hands-free activation)
- [ ] Offline map support
- [ ] Multi-language support (Hindi, regional languages)
- [ ] Admin dashboard for NGOs / rescue teams

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

```bash
# Fork the repo, create your branch, and open a PR
git checkout -b feature/your-feature-name
```

---

## 👩‍💻 Author

**Khushi Johari**
[GitHub](https://github.com/khushijohari14)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">
  <sub>Built with ❤️ for the safety of every Indian citizen.</sub>
</div>
