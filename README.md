# LYF SOS — Offline Emergency Communication App for Android

**When networks fail, humanity connects. Decentralized mesh network enabling emergency communication without internet, cellular, or cloud infrastructure.**

[![Live App](https://img.shields.io/badge/🚨%20Live%20App-lyfsos.lyfmail.com-red)](https://lyfsos.lyfmail.com)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/lyfmail-official/lyfsos/blob/main/LICENSE)
[![Privacy First](https://img.shields.io/badge/Privacy-First-blue)](https://lyfsos.lyfmail.com)
[![Android](https://img.shields.io/badge/Android-8.0%2B-brightgreen)](https://lyfsos.lyfmail.com)
[![Maintained by LYF Mail](https://img.shields.io/badge/Maintained%20by-LYF%20Mail-orange)](https://lyfmail.com)

**"People deserve emergency tools that respect them. Not louder apps. Not smarter surveillance. Just calm, honest help when it matters."**  
A free, open-source, privacy-first emergency mesh network app from [LYF Mail](https://lyfmail.com) — India's digital wellness platform.

---

## 🚨 What Is LYF SOS?

**LYF SOS** is a privacy-first, open-source **native Android emergency communication application** that creates a **decentralized mesh network** using Bluetooth Low Energy (BLE 5.0) and Wi-Fi Direct — enabling emergency communication **without internet, cellular service, or cloud infrastructure**.

Built by [LYF Mail](https://lyfmail.com), a [privacy-first digital wellness platform](https://lyfmail.com) serving 50,000+ subscribers across India since 2020, LYF SOS extends our mission of **"Every Choice Shapes Tomorrow"** into emergency preparedness and disaster resilience.

Unlike traditional emergency apps that fail when towers collapse or governments shut down networks, LYF SOS operates completely offline using **peer-to-peer mesh topology** with **end-to-end encryption** and **zero-knowledge architecture**.

---

## 🇮🇳 Why LYF SOS Exists — India-First Design

India faces unique emergency communication challenges that most global apps ignore:

- **Unstable internet connectivity** — rural areas, remote highways, and disaster zones often have zero cellular coverage.
- **Low-end Android devices** — the majority of Indians use budget phones with 2GB RAM and limited battery.
- **Battery constraints** — power outages during disasters make power-hungry apps useless.
- **Privacy concerns** — Indians rightfully distrust apps that demand phone numbers, Aadhaar, or location tracking.
- **Network shutdowns** — authoritarian internet blackouts during protests and conflicts cut off all centralized communication.
- **Natural disasters** — earthquakes, floods, and cyclones destroy cellular towers within minutes.

LYF SOS is designed specifically for these real Indian conditions. It prioritizes **reliability, dignity, and privacy over automation and surveillance**.

---

## 🔥 Core Capabilities

### 📡 Decentralized Mesh Network
LYF SOS transforms every Android phone into a network node:

- **Bluetooth LE 5.0 Broadcasting** — 100-meter range, ultra-low power consumption.
- **Wi-Fi Direct Broadcasting** — 200-meter range, higher bandwidth for detailed messages.
- **Dual-Radio Simultaneous Transmission** — maximizes discovery probability across all device types.
- **Mesh Relay with TTL Protection** — each device automatically forwards emergency packets, extending range exponentially while preventing infinite loops.

### 🔐 Zero-Knowledge Privacy Architecture
- **No accounts required** — zero phone numbers, emails, or identity verification.
- **Rotating Device IDs** — identifiers change every 15 minutes to prevent tracking.
- **End-to-End X25519 Encryption** — ephemeral keys per session, no server ever sees content.
- **Location Degradation** — precise GPS shared only with immediate neighbors; distant relays receive approximate regional data.
- **Auto-Destructing Data** — all relayed packets and temporary keys are cryptographically shredded 24 hours after emergency resolution.
- **No cloud uploads** — message content and metadata never touch a server.

### 🔋 Ultra-Low Power Design
- **&lt; 5% battery consumption per day** in mesh standby mode.
- **Adaptive Beaconing Intervals** — devices sleep intelligently when no emergency is active.
- **Android Doze Mode Respect** — works within Android's power management framework.
- **Background Mesh Participation** — your phone helps others even while in your pocket.

### 📱 Universal Android Support
- **Android 8.0+ compatible** — works on 95% of active Indian Android devices.
- **Minimum 2GB RAM required** — optimized for budget smartphones.
- **No root access needed** — standard Android permissions only.
- **No carrier dependencies** — works with any SIM or no SIM at all.

---

## 🧠 How LYF SOS Works

### Step 1: Device Discovery
When you activate an SOS signal, your device broadcasts encrypted emergency beacons via **Bluetooth Low Energy** (100m range) and **Wi-Fi Direct** (200m range) simultaneously. Nearby phones within proximity automatically detect distress signals — **no pre-configuration, no pairing, no internet required**.

### Step 2: Mesh Relay
Each receiving device automatically forwards the emergency packet to its own neighbors, creating a **multi-hop mesh network**. Messages travel across chains of devices until they reach responders, emergency contacts, or exit nodes with internet access. **Each relay extends the effective network range exponentially.**

### Step 3: Privacy Preservation
- Device IDs rotate every 15 minutes to prevent tracking.
- Location precision decreases with distance to protect sender identity.
- All messages use **end-to-end X25519 encryption** with ephemeral keys.
- No permanent identifiers stored. No conversation logs maintained.

### Step 4: Emergency Resolution
Once the emergency is resolved, all relayed data is **cryptographically shredded** within 24 hours. No traces remain on intermediate devices.

---

## 🌍 Real-World Use Cases

### 🌊 Natural Disasters
Earthquakes, floods, hurricanes, and cyclones destroy cellular towers within minutes. LYF SOS creates **instant local networks** for rescue coordination, survivor location sharing, and medical emergency triage in devastated areas where all infrastructure has failed.

### 🏔️ Remote & Rural Areas
Hiking accidents, mining incidents, farming emergencies, and rural medical crises often occur **outside cellular coverage**. LYF SOS bridges the communication gap until professional rescue arrives — perfect for India's vast rural landscape.

### 🚫 Network Shutdowns
During protests, conflicts, or authoritarian internet blackouts, governments cut internet and cellular access. LYF SOS maintains **completely independent communication channels** that no authority can shut down — because it uses no centralized infrastructure.

### 🏟️ Crowded Emergencies
Concerts, stadiums, festivals, and religious gatherings overload cellular networks with millions of simultaneous users. LYF SOS creates **local communication layers** for medical emergencies, lost person recovery, and crowd safety coordination.

### 🚑 Medical Emergencies
When someone collapses in a remote village with no ambulance service, LYF SOS can broadcast the emergency to nearby community health workers, family members, and volunteers — even without a single bar of signal.

---

## 🛡️ Core Principles

| Principle | Commitment |
|-----------|------------|
| **Privacy-First** | No tracking, no profiling, no identity collection. |
| **Consent-Based** | Nothing happens without explicit user action. |
| **No Background Surveillance** | We do not monitor, record, or track users ever. |
| **No False Promises** | Honest capability disclosure. No "guaranteed rescue" claims. |
| **No Panic-Driven UI** | Calm, clear interface designed for high-stress situations. |
| **Open-Source Transparency** | Full code auditable. No hidden services. |
| **Offline-First** | Works without internet, cellular, or cloud. |
| **Battery-Respectful** | Under 5% daily drain in standby mesh mode. |

---

## 🚫 What LYF SOS Will NEVER Do

LYF SOS has a hard ethical boundary. We will **never**:

- ❌ Track users in the background.
- ❌ Collect personal identities, phone numbers, or Aadhaar.
- ❌ Upload data silently to cloud servers.
- ❌ Run hidden services or analytics.
- ❌ Trigger SOS automatically without user consent.
- ❌ Guarantee rescue or emergency response.
- ❌ Integrate secretly with authorities or law enforcement.
- ❌ Monetize user data, attention, or metadata through advertising.
- ❌ Maintain permanent conversation logs or relay histories.
- ❌ Require accounts, logins, or identity verification.

If a feature compromises trust, it is **rejected by design**.

---

## ⚠️ Emergency Responsibility Disclaimer

**LYF SOS is NOT a replacement for official emergency services.**

In India, always attempt to contact official emergency services first:

- **112** — National Emergency Number (Police, Fire, Ambulance).
- **108** — Emergency Medical Services.
- Local police, ambulance, or fire services.

LYF SOS is a **support tool** that bridges communication gaps when infrastructure fails. It is **not a rescue guarantee**. Use it to coordinate with nearby helpers while waiting for professional emergency response.

---


## 📂 Repository Structure

```text
lyfsos/
├── app/
│   └── src/
│       ├── permissions/
│       ├── bluetooth/
│       └── location/
├── docs/
│   ├── threat-model.md
│   ├── permissions.md
│   ├── offline-behavior.md
│   ├── limitations.md
│   └── privacy.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── LICENSE
├── README.md
└── SECURITY.md
```

---

## 📄 Documentation

Every document exists to clearly explain **what the app does, what it does not do, and why certain limits exist**:

- [`docs/threat-model.md`](docs/threat-model.md) — Security threat analysis and attack vectors.
- [`docs/permissions.md`](docs/permissions.md) — Why each Android permission is requested.
- [`docs/offline-behavior.md`](docs/offline-behavior.md) — How the app behaves without connectivity.
- [`docs/limitations.md`](docs/limitations.md) — Explicit constraints and honest capability boundaries.
- [`docs/privacy.md`](docs/privacy.md) — Detailed privacy guarantees and data lifecycle.
- [`docs/mesh-protocol.md`](docs/mesh-protocol.md) — Open protocol specification for cross-platform bridging.
- [`SECURITY.md`](SECURITY.md) — Vulnerability reporting and responsible disclosure.

**Please read these documents before contributing or deploying.**

---

## 🚀 Quick Start (For Users)

### 1. Download & Install
Download the latest APK from [lyfsos.lyfmail.com](https://lyfsos.lyfmail.com) or build from source.

### 2. Grant Permissions
LYF SOS requires:
- **Location** — for GPS coordinates in emergency broadcasts.
- **Bluetooth** — for mesh network discovery and relay.
- **Wi-Fi Direct** — for extended-range mesh broadcasting.

All permissions are **explicit, documented, and used only during active emergencies**.

### 3. No Account Needed
Open the app. No phone number. No email. No signup. **Instantly ready.**

### 4. Trigger SOS in Emergency
Tap the SOS button. Your device broadcasts encrypted emergency beacons to all nearby LYF SOS users. Add an optional short message for context.

### 5. Mesh Relay Activates
Nearby devices automatically detect, decrypt, and relay your signal — extending your reach across the mesh network until help arrives.

---

## 🛠️ Development Status

| Attribute | Detail |
|-----------|--------|
| **Platform** | Android (Native). |
| **Language** | Kotlin. |
| **Minimum SDK** | Android 8.0 (API 26). |
| **Architecture** | Privacy-first, modular, offline-first. |
| **Mesh Protocol** | Bluetooth LE 5.0 + Wi-Fi Direct. |
| **Encryption** | X25519 End-to-End Ephemeral. |
| **Battery Target** | < 5% daily drain in standby. |
| **Status** | Active development. |

---

## 🤝 Contributing to LYF SOS

Contributions are welcome **only if they respect our core principles**:

- **Privacy-first design** — never compromise user privacy.
- **Explicit user consent** — no automatic triggers, no hidden behaviors.
- **Honest capability disclosure** — document what the app cannot do.
- **Non-surveillance principles** — no tracking, no profiling, no data collection.
- **India-first optimization** — budget devices, unstable networks, low battery.

Please read [`CONTRIBUTING.md`](CONTRIBUTING.md) and [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) before submitting pull requests.

---

## 🏗️ The LYF Mail Ecosystem

LYF SOS is one of nine free, open-source privacy tools built by [LYF Mail](https://lyfmail.com), a [digital wellness platform](https://lyfmail.com) from Varanasi, India, serving 50,000+ subscribers since 2020. Explore our other projects:

| Project | Description | Live App | Repository |
|---------|-------------|----------|------------|
| **[LYF Mail](https://lyfmail.com)** | Privacy-first newsletters for health, wealth, career & mindfulness. | [lyfmail.com](https://lyfmail.com) | `lyfmail` |
| **[TrustLens](https://trustlens.lyfmail.com)** | Detect misinformation before you share. Privacy-first credibility analysis. | [trustlens.lyfmail.com](https://trustlens.lyfmail.com) | `trustlens` |
| **[Signals](https://signals.lyfmail.com)** | Privacy-first analytics. Human vs. bot detection without cookies or fingerprinting. | [signals.lyfmail.com](https://signals.lyfmail.com) | `signals` |
| **[Ebb](https://ebb.lyfmail.com)** | Period tracker with homomorphic encryption. Your data stays encrypted — even from us. | [ebb.lyfmail.com](https://ebb.lyfmail.com) | `ebb` |
| **[PDPR](https://pdpr.lyfmail.com)** | Public Dark Pattern Registry. Document deceptive UX ethically. | [pdpr.lyfmail.com](https://pdpr.lyfmail.com) | `pdpr` |
| **[Together](https://together.lyfmail.com)** | Mental health support through therapeutic silence and shared presence. | [together.lyfmail.com](https://together.lyfmail.com) | `together` |
| **[Rewriter](https://lyfmail-official.github.io/rewriter/)** | AI-powered narrative therapy and health content writing assistant. | [lyfmail-official.github.io/rewriter](https://lyfmail-official.github.io/rewriter/) | `rewriter` |
| **[Offload](https://lyfmail-official.github.io/offload/)** | Stress relief with binaural beats and dream journal. Zero cloud storage. | [lyfmail-official.github.io/offload](https://lyfmail-official.github.io/offload/) | `offload` |

### 📚 Free Newsletters & Guides
- [Health & Wellness Guide](https://lyfmail.com/health-wellness-guide)
- [Personal Finance Guide](https://lyfmail.com/personal-finance-guide)
- [Career Development Guide](https://lyfmail.com/career-development-guide)
- [Creativity Resources](https://lyfmail.com/creativity-resources)
- [Mindfulness Practices](https://lyfmail.com/mindfulness-practices)

**Newsletter Signups:** [Health](https://health.signup.lyfmail.com) · [Finance](https://financing.signup.lyfmail.com) · [Career](https://career.signup.lyfmail.com) · [Creativity](https://creativity.signup.lyfmail.com) · [Personal Development](https://intuition.signup.lyfmail.com)

---

## 📜 License

LYF SOS is released under the **MIT License**.

You are free to use, modify, and distribute it — including commercially. See [`LICENSE`](LICENSE) for full terms.

---

## 📫 Connect With Us

- **🌐 Website:** [lyfmail.com](https://lyfmail.com)
- **🚨 LYF SOS App:** [lyfsos.lyfmail.com](https://lyfsos.lyfmail.com)
- **📱 PWA:** [app.lyfmail.com](https://app.lyfmail.com)
- **📚 Documentation:** [docs.lyfmail.com](https://docs.lyfmail.com)
- **🎨 Brand Assets:** [github.com/lyfmail-official/lyfmail-brand-assets](https://github.com/lyfmail-official/lyfmail-brand-assets)
- **🐦 X / Twitter:** [LYF Mail](https://x.com/lyfmailcom)
- **📘 Facebook:** [LYF Mail](https://www.facebook.com/thelyfmail)
- **▶️ YouTube:** [LYF Mail](https://m.youtube.com/channel/UCurymhWrl2nkvv31uJMuc0g)
- **💼 LinkedIn:** [LYF Mail](https://www.linkedin.com/company/lyf-mail)
- **📧 Email:** contact@lyfmail.com
- **🆘 Support:** [support.lyfmail.com](https://support.lyfmail.com)

---

> *"Every Choice Shapes Tomorrow"*

**Maintained by [LYF Mail](https://lyfmail.com)** · Founded by [Ajay Kumar Chaudhary](https://github.com/lyfmail) · Varanasi, Uttar Pradesh, India · Since 2020

---

## 💬 Frequently Asked Questions

**Q: How does LYF SOS work without internet or cellular service?**  
A: LYF SOS uses your phone's built-in Bluetooth Low Energy and Wi-Fi Direct radios to create a decentralized mesh network. When you activate an SOS signal, your device broadcasts encrypted packets that nearby phones detect and automatically relay forward. Each relay extends the network range, allowing messages to travel kilometers across a chain of devices without ever touching the internet or cellular infrastructure.

**Q: Is LYF SOS completely free and open source?**  
A: Yes. LYF SOS is released under the MIT License and available on GitHub. There are no in-app purchases, no premium tiers, and no advertising. The project is maintained by volunteers and supported by the LYF Mail privacy advocacy community.

**Q: What is the maximum communication range?**  
A: Direct device-to-device range is approximately 100 meters for Bluetooth LE and 200 meters for Wi-Fi Direct in open conditions. However, the mesh network extends this exponentially — each device that receives and relays a message becomes a new broadcast point. In dense urban environments with hundreds of participating devices, effective network coverage can span several kilometers.

**Q: How does LYF SOS protect my privacy and identity?**  
A: LYF SOS implements a zero-knowledge architecture. Device identifiers rotate every 15 minutes to prevent tracking. Location data is deliberately degraded with distance — precise GPS is shared only with immediate neighbors, while distant relays receive approximate regional data. All messages use end-to-end X25519 encryption with ephemeral keys that are destroyed after delivery. No account creation means no linkable identity.

**Q: Will LYF SOS drain my battery if I keep it installed?**  
A: No. In standby mesh mode, LYF SOS consumes less than 5% battery per day. The app uses adaptive beaconing — when no emergency is active, devices enter a low-power listening state with periodic wake intervals. During an active emergency relay, power consumption increases temporarily but respects Android Doze mode and app standby optimizations to minimize impact.

**Q: Can LYF SOS be used for non-emergency communication?**  
A: LYF SOS is specifically designed and optimized for emergency scenarios. While the underlying mesh protocol could theoretically support general messaging, the application intentionally restricts usage to distress signals, medical emergencies, and disaster coordination to prevent network congestion and maintain the ethical integrity of the emergency spectrum.

**Q: Does LYF SOS work on all Android phones?**  
A: LYF SOS requires Android 8.0 or higher and a minimum of 2GB RAM. It is compatible with 95% of active Android devices in India, including budget smartphones. No root access or special hardware is required.

**Q: Is LYF SOS available on Google Play Store?**  
A: LYF SOS is distributed directly via [lyfsos.lyfmail.com](https://lyfsos.lyfmail.com) and GitHub releases to avoid Play Store tracking requirements and maintain our privacy-first commitment. You can download the APK directly and install it on any compatible Android device.

**Q: Can iOS users join the LYF SOS mesh network?**  
A: The current release is Android-only. However, our mesh protocol specifications are published openly in `docs/mesh-protocol.md`, enabling iOS and embedded device implementations to join the same mesh network in the future.

**Q: What happens to my data after an emergency?**  
A: All relayed packets and temporary encryption keys are cryptographically shredded within 24 hours of emergency resolution. No permanent logs, no conversation history, no metadata retention. Your emergency data simply ceases to exist.

---

*This README is maintained by the LYF Mail team. For issues, feature requests, security reports, or contributions, please visit our [GitHub repository](https://github.com/lyfmail-official/lyfsos).*

**Maintained by [LYF Mail](https://github.com/lyfmail-official)** · 
Founded by [Ajay Kumar Chaudhary](https://github.com/lyfmail) 

