# Limitations — LYF SOS (Android)

This document clearly states the **technical, ethical, and practical limitations**
of the LYF SOS Android application.

LYF SOS is designed to **assist during emergencies**, not to replace official
emergency services, hardware devices, or guaranteed rescue systems.

Honesty about limitations is a core safety principle.

---

## 🎯 Purpose of This Document

- Prevent false expectations.
- Avoid dangerous assumptions.
- Maintain ethical transparency.
- Protect users in real emergencies.
- Ensure platform compliance (Google Play, FOSS norms).

---

## 🚨 Not a Replacement for Emergency Services

LYF SOS:

- ❌ Is NOT a replacement for police, ambulance, fire, or disaster services.
- ❌ Does NOT automatically contact government emergency numbers.
- ❌ Does NOT guarantee message delivery or response.

Users must **always prioritize calling official emergency numbers** when possible.

---

## 📶 Network Dependency Limitations

### Internet Availability

When internet is unavailable:

- SOS messages cannot be sent online.
- Location sharing may be delayed or unavailable.
- Delivery confirmation is impossible.

LYF SOS does **not**:
- Auto-retry sending messages.
- Queue messages for later transmission.
- Send alerts silently when connectivity returns.

---

## 📍 Location Accuracy Limitations

Location data may be:

- Delayed.
- Approximate.
- Unavailable indoors or underground.
- Based on last-known GPS fix.

LYF SOS does not:
- Use cell tower triangulation without permission.
- Improve accuracy using background tracking.
- Store historical location data.

Location accuracy depends entirely on:
- Device hardware.
- Satellite visibility.
- User permissions.

---

## 🔋 Battery & Device Constraints

LYF SOS performance may be limited by:

- Low battery levels.
- Power-saving modes.
- OS-level background restrictions.
- Manufacturer-specific Android modifications.

The app avoids:
- Continuous background services.
- Persistent wake locks.
- Battery-draining operations.

This may reduce real-time responsiveness in some situations.

---

## 📡 Bluetooth & Offline Limitations

If Bluetooth-based features are enabled:

- Range is limited (typically under 100 meters).
- Obstructions may block signals.
- Device compatibility varies.
- Reliability is not guaranteed in crowded environments.

Bluetooth is:
- Optional.
- User-controlled.
- Not always active.

---

## 🧠 Human Factors

LYF SOS cannot account for:

- User panic or incorrect input.
- Incomplete messages.
- Disabled permissions.
- Misuse or accidental activation.

The app intentionally avoids:
- Panic-inducing UI.
- Forced workflows.
- Automatic behavior without consent.

---

## 🔐 Security & Threat Limitations

While LYF SOS follows strong security practices:

- No system is completely immune to attacks.
- Compromised devices may leak data.
- Rooted or modified devices may bypass protections.

LYF SOS does not:
- Perform device integrity checks.
- Block rooted devices.
- Enforce encryption beyond OS-level guarantees.

---

## 🏛️ Legal & Jurisdictional Limitations

Emergency handling laws vary by country and region.

LYF SOS:
- Does not adapt behavior based on local emergency laws.
- Does not integrate with government emergency systems.
- Makes no legal guarantees regarding compliance or outcomes.

Users are responsible for understanding local emergency procedures.

---

## 🚫 Features LYF SOS Intentionally Does NOT Provide

- Background tracking.
- Continuous location monitoring.
- Auto SOS triggers.
- AI-based emergency detection.
- Social media broadcasting.
- Law enforcement integrations.

These exclusions are **intentional design decisions**, not missing features.

---

## 📌 Transparency Commitment

LYF SOS commits to:

- Documenting limitations clearly.
- Never exaggerating capabilities.
- Never claiming guaranteed safety.
- Never misleading users during emergencies.

---

## 📋 Summary Table

| Area | Limitation |
|----|----|
| SOS Delivery | Not guaranteed |
| Internet | Required for online alerts |
| GPS | Accuracy varies |
| Bluetooth | Short range |
| Background Operation | Not supported |
| Legal Coverage | None guaranteed |

---

## 🔗 Related Documents

- `docs/threat-model.md`
- `docs/permissions.md`
- `docs/offline-behavior.md`
- `SECURITY.md`
- `README.md`

---

**Emergency tools must be honest, predictable, and minimal.**

LYF SOS chooses transparency over false reassurance.
