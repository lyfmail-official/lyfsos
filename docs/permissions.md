# Permissions — LYF SOS (Android)

This document explains **why LYF SOS requests specific Android permissions**, how they are used, and what is explicitly **not** done with them.

LYF SOS follows a **minimum-permissions principle**.

No permission is requested unless it directly supports an emergency feature.

---

## 🎯 Design Philosophy

- Permissions are requested **only when needed**.
- No permission is required at install time.
- All sensitive permissions are **user-triggered**.
- The app remains usable even if permissions are denied.
- No background access to sensitive data.

---

## 📍 Location Permission

### Permission
- `ACCESS_FINE_LOCATION`
- `ACCESS_COARSE_LOCATION`

### Purpose
- Capture current location **only during an SOS event**.
- Allow user to share approximate or precise location manually.

### Usage Rules
- Requested only when user taps SOS.
- Used once per SOS action.
- No background tracking.
- No location history stored.
- No silent access.

### If Denied
- SOS still works.
- User can send text-only SOS message.

---

## 📶 Bluetooth Permission (Optional)

### Permission
- `BLUETOOTH`
- `BLUETOOTH_CONNECT` (Android 12+)

### Purpose
- Optional nearby-device signaling (future / experimental).
- No continuous scanning.

### Usage Rules
- Disabled by default.
- Foreground-only usage.
- User must explicitly enable.
- No device identifiers stored.

### If Denied
- Feature is skipped without errors.

---

## 📞 Phone / SMS Permissions

### Permission
- **None requested by default**

### Notes
- LYF SOS does NOT auto-send SMS.
- Sharing is done via Android system share sheet.
- The user selects the communication app manually.

This avoids misuse and accidental alerts.

---

## 📁 Storage Permissions

### Permission
- **None (Scoped Storage only)**

### Purpose
- Temporary local storage of SOS message draft.

### Usage Rules
- App-private storage only.
- Automatically deleted on uninstall.
- No media scanning.
- No external storage access.

---

## 📷 Camera / Microphone

### Permission
- **Not requested**

### Notes
- No audio recording.
- No video capture.
- No background listening.
- No image capture.

---

## 🌐 Internet Permission

### Permission
- `INTERNET`

### Purpose
- Optional link previews.
- Optional emergency resource links.
- Update static safety information.

### Usage Rules
- No analytics.
- No telemetry.
- No background network calls.
- No auto-transmission of SOS data.

---

## 🚫 Explicitly NOT Requested

LYF SOS will never request:

- Contacts access.
- Call logs.
- SMS read/write.
- Background location.
- Accessibility services.
- Device ID / IMEI.
- Advertising ID.
- Usage stats.
- Overlay permissions.

---

## 🔍 Permission Transparency

- Every permission is documented.
- Permission prompts explain **why**.
- No misleading permission text.
- No conditional dark patterns.

Users remain in control.

---

## ⚠️ Risk Disclosure

Denying permissions may reduce functionality, but:
- The app will not crash.
- The user will be informed.
- The decision is respected.

Emergency software must **never coerce consent**.

---

## 📌 Summary Table

| Permission | Required | When Used | Purpose |
|----------|--------|----------|--------|
| Location | Optional | SOS action | Share user location |
| Bluetooth | Optional | Manual enable | Nearby signaling |
| Internet | Optional | Foreground | Resource access |

---

## 🔗 Related Documents

- `docs/threat-model.md`
- `docs/privacy.md`
- `docs/offline-behavior.md`
- `docs/limitations.md`

