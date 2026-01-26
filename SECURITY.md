# Security Policy — LYF SOS (Android)

LYF SOS is a privacy-first, open-source native Android emergency support app.
Security is treated as a **design constraint**, not an afterthought.

This document explains how security is handled and how vulnerabilities should be reported.

---

## 📌 Scope

This security policy applies to:

- LYF SOS Android application source code.
- Local data storage mechanisms.
- Permission handling and enforcement.
- Bluetooth / Wi-Fi Direct modules (where enabled).
- Offline data queues.
- Build and release configurations.

It does NOT apply to:
- Forks with modified security logic.
- Repackaged APKs.
- Third-party builds.

---

## 🔐 Security Principles

LYF SOS follows these core security principles:

- **Least privilege** — request only what is necessary.
- **User control** — no background actions without consent.
- **Local-first data handling**.
- **No central server dependency**.
- **No silent network activity**.
- **Explicit user awareness**.

Security should never rely on obscurity.

---

## 💾 Data Security

### Local Storage
- All emergency data is stored **locally on the device**.
- Uses Android-provided storage APIs.
- No cloud sync.
- No remote backups by default.

### Data Lifetime
- Data exists only until:
  - User deletes it.
  - App is uninstalled.
  - Device storage is cleared.

---

## 🌐 Network Security

- No persistent background connections.
- No telemetry or analytics endpoints.
- No WebSockets or background sync.
- Network activity occurs only when:
  - User explicitly shares SOS information.
  - User initiates communication.

LYF SOS does not maintain servers that receive user emergency data.

---

## 📡 Bluetooth & Local Communication

When enabled:

- Bluetooth operates only in **foreground mode**.
- No continuous scanning in background.
- No automatic peer discovery.
- No unique device identifiers are broadcast.
- User must explicitly enable Bluetooth features.

All local communication is designed to be **ephemeral and opt-in**.

---

## 🔑 Permissions Enforcement

- Permissions are requested **at runtime**.
- Each permission is tied to a visible user action.
- App remains usable with partial permissions.
- No permission escalation tricks are used.

Full details are documented in `docs/permissions.md`.

---

## 🧠 Threat Model Awareness

LYF SOS acknowledges the following out-of-scope threats:

- Compromised Android OS.
- Rooted devices with malicious software.
- Physical access to unlocked devices.
- Manufacturer-level backdoors.

See `docs/threat-model.md` for detailed analysis.

---

## 🧪 Supported Versions

| Version | Security Support |
|-------|------------------|
| Latest stable release | ✅ Yes |
| Development branches | ⚠️ Best effort |
| Old releases | ❌ No |

Only the latest release receives active security attention.

---

## 🚨 Reporting a Vulnerability

If you discover a security issue:

1. **DO NOT open a public GitHub issue**
2. Email details to: **help@lyfmail.com**
3. Include:
   - Description of the issue.
   - Steps to reproduce.
   - Affected Android versions/devices.
   - Potential impact.

We aim to acknowledge reports within **72 hours**.

---

## 🤝 Responsible Disclosure

- Please allow reasonable time to address issues.
- Coordinated disclosure is appreciated.
- Public disclosure before a fix may put users at risk.

---

## 💰 Bug Bounty

There is **no paid bug bounty program**.
This is a public-interest, non-commercial project.

Valid reports are still deeply appreciated.

---

## ⚠️ Disclaimer

LYF SOS is **not a certified life-critical system**.

The software is provided **“AS IS”**, without warranty of any kind.
Users must rely on official emergency services when available.

---

## ❤️ Final Note

Security is about **trust, clarity, and restraint**.

If a feature compromises user trust, it does not belong in LYF SOS.
