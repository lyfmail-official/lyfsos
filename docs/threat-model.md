# Threat Model — LYF SOS (Android)

This document describes the **security threat model** for the LYF SOS native Android application.

The goal is not to claim perfect security, but to **explicitly define risks, boundaries, and mitigations**.

---

## 🎯 Purpose

- Identify realistic threats to users.
- Clarify what LYF SOS protects against.
- Clearly state what is **out of scope**.
- Prevent false assumptions about safety or guarantees.

Emergency software must be **transparent about risk**.

---

## 🧱 Assets to Protect

LYF SOS aims to protect:

- User-generated SOS messages.
- User location data (during SOS only).
- User intent (prevent silent actions).
- Application integrity.
- User trust.

LYF SOS does **not** handle identities, accounts, or credentials.

---

## 👤 Threat Actors

### 1️⃣ Malicious Applications
- Other apps on the same device attempting data access.
- Apps abusing Android permissions.

### 2️⃣ Network Adversaries
- Intercepting traffic during data sharing.
- Man-in-the-middle attacks on public networks.

### 3️⃣ Physical Access Attackers
- Access to unlocked devices.
- Temporary access during emergencies.

### 4️⃣ Malicious Forks
- Modified versions falsely claiming official support.
- Repackaged APKs.

---

## 🧨 Identified Threats & Mitigations

### 🔓 Unauthorized Data Access
**Threat:** Other apps accessing SOS data  .
**Mitigation:**
- Use Android sandboxed storage.
- No exported content providers.
- No world-readable files.

---

### 📡 Network Interception
**Threat:** SOS data intercepted during sharing  .
**Mitigation:**
- No automatic network transmission.
- User-controlled sharing via trusted apps.
- HTTPS enforced where applicable.

---

### 🕵️ Background Surveillance
**Threat:** App secretly tracking user behavior  .
**Mitigation:**
- No background services.
- No hidden workers.
- No analytics or telemetry.

---

### 🧬 Bluetooth Misuse
**Threat:** Device fingerprinting or tracking  .
**Mitigation:**
- No persistent device identifiers.
- Foreground-only Bluetooth usage.
- User-controlled activation.

---

### 🗃️ Data Persistence Abuse
**Threat:** Old SOS data lingering on device  .
**Mitigation:**
- Clear data options.
- Automatic cleanup on uninstall.
- User-visible storage behavior.

---

### 🧑‍💻 Supply Chain Attacks
**Threat:** Malicious dependency injection  .
**Mitigation:**
- Minimal dependencies.
- Open-source review.
- No closed-source SDKs.

---

## 🚫 Out-of-Scope Threats

LYF SOS does **not** attempt to mitigate:

- Rooted or compromised Android OS.
- Manufacturer-installed malware.
- Hardware backdoors.
- Advanced nation-state surveillance.
- Physical attacks on the user.
- Denial of service from lack of connectivity.

These are beyond the app’s control.

---

## ⚠️ Risk Acceptance

Certain risks are accepted intentionally:

- Reliance on Android OS security.
- Reliance on user judgment during emergencies.
- Dependence on third-party apps for message delivery.

The alternative would require intrusive control, which is rejected.

---

## 🧭 Ethical Security Boundaries

LYF SOS will **not**:

- Monitor users continuously.
- Automate emergency decisions.
- Track location in background.
- Override user consent.
- Sacrifice privacy for automation.

Security must respect dignity.

---

## 📌 Summary

LYF SOS security is:
- Local-first.
- User-controlled.
- Transparent.
- Conservative by design.

Understanding limitations is part of staying safe.

---

## 🔗 Related Documents

- `SECURITY.md`
- `docs/permissions.md`
- `docs/offline-behavior.md`
- `docs/limitations.md`
- `docs/privacy.md`

