# 🏠 My Home Security Setup

A practical approach to securing a multi-device home network with separate work/personal environments.

---

## 📌 Overview

This document outlines my personal home security setup, including network configuration, device management, password security, 2FA, backups, secure communication, endpoint protection, and lessons learned from real security incidents.

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

### Virtual Lab Environment
- **Hypervisor**: Oracle VirtualBox
- **Guest OS**: Ubuntu, Kali Linux
- **Purpose**: Cybersecurity training, penetration testing practice, secure experimentation

### Device Count
- 3 phones
- 3 laptops
- 1 tablet
- 1 external monitor
- 2 virtual machines (Ubuntu, Kali)

---

## 🛡️ Endpoint Protection

### Windows Devices (All Laptops)
- **Windows Defender Firewall**: Enabled (default configuration)
- **Windows Security**: Real-time protection, cloud-delivered protection, automatic sample submission
- **Avira Antivirus**: Additional layer of protection on all Windows laptops

### Mobile Devices
- **Android**: Google Play Protect (built-in)
- **iOS**: Built-in security features, app sandboxing

### Security Track Record
- **Mobile devices**: No security breaches in 20+ years (Android, iOS)
- **Home network**: No security breaches in 2+ years
- **Work network (Ubuntu server, laptops)**: No security breaches in 2+ years
- **All connected devices**: No compromises since the 2023 incident (see below)

---

## 🧠 Security Awareness & Safe Practices

### NEVER:
- Open links received via SMS
- Open unsolicited emails from unknown senders
- Click any link in emails (zero exceptions)
- Download attachments from unknown sources
- Visit unverified websites or pages flagged by Google security alerts
- Install software that downloads automatically
- Install anything without explicit management approval

### ALWAYS:
- Inform my partner about new phishing methods (e.g., fake parcel delivery SMS, "update your address" scams)
- Let her show me anything she's unsure about
- Double-check suspicious items with AI verification tools
- Use separate emails for different purposes:
  - Work email
  - Personal email
  - YouTube / social media email (this one receives phishing attempts daily)

---

## 📌 Real Incident & Lessons Learned

### Breach (2 years ago — 2023)
- **Cause**: Downloaded a modified version of a drawing program from a YouTube link
- **Mistake**: Ignored Windows Security alerts during installation
- **Impact**: Malware infection
- **Response**: Changed hundreds of passwords, reinstalled Windows, fully cleaned the system

### Key Lessons:
- No software from untrusted sources, even if it looks legitimate
- Never ignore security alerts — they exist for a reason
- Even open-source software can be compromised when downloaded from unofficial sources
- Regular advanced scans with tools like CCleaner and Avira Pro help identify subtle threats missed by basic protection

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
- **Avira**: Automatic updates enabled
- **Router**: Updates handled automatically by ISP
- **Virtual machines**: Updated regularly (Ubuntu, Kali)

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
9. **Defense in depth** – Windows Firewall + Windows Security + Avira on all laptops
10. **Virtual lab** – Safe environment for testing and learning
11. **Proven track record** – No mobile breaches in 20+ years; no network breaches in 2+ years

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
| [security-timeline.md](docs/security-timeline.md) | Security history and lessons learned |
| [nmap-scan.png](images/nmap-scan.png) | Screenshot of network scan |
| [router.jpg](images/router.jpg) | Router photo |
| [virtualbox-lab.png](images/virtualbox-lab.png) | VirtualBox lab setup |

---

## 📅 Last Updated

March 2026
