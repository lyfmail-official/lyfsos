# Offline Behavior — LYF SOS (Android)

This document explains how **LYF SOS behaves when the device has no internet
connection**, poor connectivity, or restricted network access.

LYF SOS is designed to function in **real-world emergency conditions**, where
network availability cannot be assumed.

---

## 🎯 Core Principle

> **Emergency assistance must never depend on internet access.**

LYF SOS prioritizes:
- Offline usability.
- Predictable behavior.
- Zero failures during connectivity loss.

---

## 📵 Offline-First Design

LYF SOS works in the following conditions:

- No mobile data.
- No Wi-Fi.
- Airplane mode (partial functionality).
- Network blocked or throttled.
- Captive portals (railways, public Wi-Fi).

The app **does not freeze, crash, or silently fail**.

---

## 🚨 SOS Trigger Behavior (Offline)

### When User Presses SOS (Offline)

- SOS screen activates immediately.
- Local emergency message is prepared.
- Location access is attempted (GPS-only, no network).
- User is clearly informed of offline state.

### What Still Works
- Manual message composition.
- GPS-based location (if satellites available).
- Copy SOS message to clipboard.
- Share via any locally available app (SMS app, offline Bluetooth share, etc.).

### What Is Skipped
- Online link previews.
- External emergency resource fetching.
- Any cloud-dependent features.

---

## 📍 Location Handling Offline

### Behavior
- Uses device GPS only.
- No cell-tower triangulation.
- No Wi-Fi-based positioning.

### Outcomes
- Location may take longer to acquire.
- Accuracy may vary.
- Last-known location may be used (with user notice).

### Transparency
The user is always informed if:
- Location is unavailable.
- Location is approximate.
- Location data is stale.

---

## 📶 Bluetooth (Offline)

If enabled by the user:

- Bluetooth works without internet.
- Used only for nearby signaling (if implemented).
- No continuous scanning.
- No background operation.

Bluetooth remains **entirely optional**.

---

## 📁 Local Storage Behavior

### What Is Stored Locally
- Temporary SOS draft message.
- App configuration settings.

### What Is NOT Stored
- Location history.
- Past SOS events.
- User identity data.
- Analytics logs.

### Cleanup
- Temporary data cleared after SOS completion.
- All data removed on uninstall.

---

## 🔁 Retry & Recovery

When connectivity returns:

- App does **not auto-send** any data.
- User must manually retry or resend.
- No background retries.
- No queued transmissions.

This prevents accidental or delayed alerts.

---

## 🧭 User Communication

LYF SOS clearly communicates:

- Offline status indicators.
- Reduced functionality warnings.
- Available actions while offline.

No silent degradation.

---

## 🚫 What LYF SOS Will NEVER Do Offline

- Attempt hidden network calls.
- Cache emergency messages for later sending.
- Automatically send data when internet returns.
- Use background services to retry SOS.

User intent is always required.

---

## ⚠️ Limitations Acknowledged

Offline mode **cannot**:
- Contact emergency services automatically.
- Verify message delivery.
- Fetch live emergency numbers.

These limitations are openly documented.

---

## 📌 Summary Table

| Feature | Offline Support |
|------|----------------|
| SOS Trigger | ✅ Yes |
| Manual Message | ✅ Yes |
| GPS Location | ✅ (Satellite only) |
| Bluetooth | ✅ Optional |
| Internet Features | ❌ Disabled |
| Auto-Send | ❌ Never |

---

## 🔗 Related Documents

- `docs/permissions.md`
- `docs/threat-model.md`
- `docs/privacy.md`
- `docs/limitations.md`

---

**Offline safety is not a fallback — it is the default.**

LYF SOS is built for reality, not ideal conditions.
