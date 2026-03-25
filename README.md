# 🏠 My Home Security Setup

A practical approach to securing a multi-device home network with separate work/personal environments.

---

## 📌 Overview

This document outlines my personal home security setup, including network configuration, device management, password security, 2FA, backups, and secure communication.

---

## 🔧 Hardware & Network Infrastructure

### Internet Provider
- **Provider**: Primnet (fiber optic)
- **Connection**: Stable, high-speed fiber

### Router
- **Model**: ZTE ZXHN H2680
- **Provider-managed**: Configuration via ISP mobile app
- **Security**: Management interface not exposed to LAN (ISP restriction)
- **Firmware updates**: Handled automatically by ISP
- **WiFi Security**: WPA3 (configured via ISP app)

### Network Devices

| Device | Type | OS | Role |
|--------|------|-----|------|
| Samsung Galaxy S25 Ultra | Phone | Android | Daily driver |
| iPhone 13 Pro Max | Phone | iOS | Secondary |
| Samsung Galaxy Flip 3 | Phone | Android | Partner's device |
| HP Laptop (Intel i5 + NVIDIA) | Laptop | Windows | Study / VM lab |
| Lenovo Laptop (Ryzen) | Laptop | Windows | Work |
| HP Laptop | Laptop | Windows | Backup / Media |
| Lenovo Tablet | Tablet | Android | Partner's media |
| Philips 278E | Monitor | - | External display |

### Device Count
- 3 phones
- 3 laptops
- 1 tablet
- 1 external monitor

---

## 🔐 Authentication & Access Control

- **All mobile devices**: Fingerprint enabled
- **All laptops**: Fingerprint / Windows Hello enabled
- **All devices**: Protected with strong, unique passwords
- **No password reuse** across devices

---

## 🔑 Password & 2FA Management

### Password Manager
- **Tool**: Standard Notes (end-to-end encrypted)
- **Notes**: Work passwords, Personal passwords, Partner's passwords
- **Synced devices**: S25 Ultra, iPhone 13, Flip 3

### Two-Factor Authentication (2FA)
- **Tool**: Google Authenticator
- **Synced across**: 3 mobile devices
- **All critical accounts**: Protected with 2FA

### Account Separation

| Device | Accounts |
|--------|----------|
| Work laptop | Work only |
| Study laptop | Personal only |
| Media laptop | Personal only |
| Personal phones | Personal + shared work notes |
| Partner's phone | Her personal accounts + shared work notes |

---

## 💬 Secure Communication

- **Tool**: Signal (end-to-end encrypted)
- **Used for**: Work-related communication
- **Platforms**: All 3 mobile devices

---

## 💾 Backup Strategy

- **External HDD**: 1TB
- **Frequency**: Manual, minimum once per week
- **Content**: No major weekly changes

---

## 🔄 Update Management

- **All devices**: Manual updates triggered by notifications
- **Windows/Android/iOS**: Updated when notified
- **Router**: Updates handled automatically by ISP

---

## 🔒 Physical Security

- No unauthorized physical access to devices
- No external guests on the network
- All devices locked when unattended

---

## 📱 Cross-Device Sync

| Service | Synced Devices | Purpose |
|---------|----------------|---------|
| Standard Notes | S25 Ultra, iPhone 13, Flip 3 | Passwords, work codes |
| Google Authenticator | 3 mobile devices | 2FA codes |
| Signal | 3 mobile devices | Secure communication |

---

## 🧠 Lessons Learned

1. **Separation is key** – Work and personal data never mix
2. **Password manager** – E2EE without relying on big tech
3. **2FA across devices** – Redundancy if one device is lost
4. **Secure communication** – Signal for sensitive chats
5. **Regular backups** – Manual but consistent
6. **ISP-managed router** – Adds a layer of security (no local web access)
7. **Biometric everywhere** – Fast, secure access
8. **Strong unique passwords** – No reuse across devices

---

## 🔮 Future Improvements

- [ ] VPN on router (if ISP allows)
- [ ] DNS over HTTPS (Cloudflare 1.1.1.1)
- [ ] Network traffic monitoring
- [ ] Hardware security key (YubiKey)
- [ ] Automated backup script

---

## 📄 Files in this repository

| File | Description |
|------|-------------|
| [README.md](README.md) | This document |
| [router-settings.md](router-settings.md) | Router configuration notes |
| [security-checklist.md](security-checklist.md) | Weekly security checklist |
| [nmap-scan.png](images/nmap-scan.png) | Screenshot of network scan |
| [router.jpg](images/router.jpg) | Router photo |

---

## 📅 Last Updated

March 2026
