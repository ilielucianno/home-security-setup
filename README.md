# 🏠 My Home Security Setup

A practical approach to securing a multi-device home network with separate work/personal environments.

---

## 📌 Overview

This document outlines my personal home security setup, including network configuration, device management, password security, 2FA, backups, secure communication, endpoint protection, and lessons learned from real security incidents.

---

## 🔧 Hardware & Network Infrastructure

### Internet Provider
- **Provider**: Fiber optic ISP PRIMETEL
- **Connection**: Stable, high-speed fiber

### Router
- **Model**: ISP-provided router HUAWEI
- **Provider-managed**: Configuration via ISP mobile app
- **Security**: Management interface not exposed to LAN (ISP restriction)
- **Firmware updates**: Handled automatically by ISP
- **WiFi Security**: WPA3 (configured via ISP app)

### Network Devices (General Description)

| Type | Count | Role |
|------|-------|------|
| Smartphones | Multiple | Personal and work communication |
| Laptops | Multiple | Work, study, media |
| Tablet | 1 | Media consumption |
| External monitor | 1 | Extended display for study setup |

### Virtual Lab Environment
- **Hypervisor**: Oracle VirtualBox
- **Guest OS**: Ubuntu, Kali Linux
- **Purpose**: Cybersecurity training, penetration testing practice, secure experimentation

---

## 🛡️ Endpoint Protection

### Windows Devices
- **Windows Defender Firewall**: Enabled
- **Windows Security**: Real-time protection, cloud-delivered protection
- **Avira Antivirus**: Additional layer of protection

### Mobile Devices
- **Android**: Google Play Protect (built-in)
- **iOS**: Built-in security features

### Security Track Record
- **Mobile devices**: No security breaches in 20+ years
- **Home network**: No security breaches in 2+ years
- **Work network**: No security breaches in 2+ years
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
  - Social media email

---

## 📌 Real Incident & Lessons Learned

### Breach (2 years ago)
- **Cause**: Downloaded a modified version of a legitimate program from a YouTube link
- **Mistake**: Ignored Windows Security alerts during installation
- **Impact**: Malware infection
- **Response**: Changed all passwords, reinstalled Windows, fully cleaned the system

### Key Lessons:
- No software from untrusted sources, even if it looks legitimate
- Never ignore security alerts — they exist for a reason
- Even open-source software can be compromised when downloaded from unofficial sources
- Regular advanced scans help identify subtle threats missed by basic protection

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
- **Synced devices**: Multiple mobile devices

### Two-Factor Authentication (2FA)
- **Tool**: Google Authenticator
- **Synced across**: Multiple mobile devices
- **All critical accounts**: Protected with 2FA

### Account Separation

| Device Type | Accounts |
|-------------|----------|
| Work laptop | Work only |
| Study laptop | Personal only |
| Media laptop | Personal only |
| Personal phones | Personal + shared work notes |
| Partner's phone | Her personal accounts + shared work notes |

---

## 💬 Secure Communication

- **Tool**: Signal (end-to-end encrypted)
- **Used for**: Work-related communication
- **Platforms**: Mobile devices

---

## 💾 Backup Strategy

- **External HDD**: Regular manual backups
- **Frequency**: Minimum once per week
- **Content**: No major weekly changes

---

## 🔄 Update Management

- **All devices**: Manual updates triggered by notifications
- **Windows/Android/iOS**: Updated when notified
- **Avira**: Automatic updates enabled
- **Router**: Updates handled automatically by ISP
- **Virtual machines**: Updated regularly

---

## 🔒 Physical Security

- No unauthorized physical access to devices
- No external guests on the network
- All devices locked when unattended

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
9. **Defense in depth** – Multiple security layers
10. **Virtual lab** – Safe environment for testing and learning
11. **Proven track record** – Long history of no security breaches

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

---

**Ilie Lucian**  
Technical Department Manager with 10+ years in IT infrastructure, networking, and hardware. Currently pursuing certifications in cybersecurity (TryHackMe SEC1, Security+, Network+).

### Why I Built This
I've been working in IT infrastructure for 10+ years, managing networks, hardware, and teams. Recently, I realized that what I was already doing (firewalls, VLANs, VPNs, incident response) has a name: **cybersecurity**. Now I'm formalizing my knowledge through certifications and documenting real projects to demonstrate my skills.

**This repository is a living document of my cybersecurity journey.**

## 📅 Last Updated
March 2026
