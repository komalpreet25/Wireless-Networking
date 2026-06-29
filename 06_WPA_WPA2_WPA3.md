# WPA, WPA2, WPA3 (Wi-Fi Security)

## Description

WPA, WPA2, and WPA3 are Wi-Fi security protocols used to protect wireless networks from unauthorized access.

They define how encryption, authentication, and data protection are handled in Wi-Fi communication.

These protocols evolved to fix weaknesses in older security systems like WEP.

---

# Why Wi-Fi Security is Needed

Wireless networks are vulnerable because:

* Signals travel through air
* Anyone nearby can capture packets
* Unauthorized users can try to connect
* Data can be intercepted

Wi-Fi security protocols protect:

* Data privacy
* Network access
* User authentication

---

# Evolution of Wi-Fi Security

| Standard | Year | Security Level |
| -------- | ---- | -------------- |
| WEP      | 1997 | Weak (Broken)  |
| WPA      | 2003 | Improved       |
| WPA2     | 2004 | Strong         |
| WPA3     | 2018 | Strongest      |

---

# 1. WEP (Wired Equivalent Privacy)

## Features

* First Wi-Fi security protocol
* Uses RC4 encryption

## Problems

* Weak encryption
* Easily cracked
* Not secure anymore

## Status

```text id="wep1"
DEPRECATED (NOT SAFE)
```

---

# 2. WPA (Wi-Fi Protected Access)

Introduced as an improvement over WEP.

## Features

* Uses TKIP encryption
* Dynamic key generation
* Better security than WEP

## Weaknesses

* Still vulnerable to attacks
* Replaced by WPA2

---

# 3. WPA2

WPA2 is the most widely used Wi-Fi security standard.

## Features

* Uses AES encryption
* Strong security
* Mandatory for Wi-Fi certification

---

## Encryption: AES

AES stands for:

```text id="aes1"
Advanced Encryption Standard
```

Benefits:

* Strong encryption
* Widely trusted
* Used in government and enterprise systems

---

## WPA2 Modes

### WPA2-Personal

* Uses password (Pre-Shared Key)
* Common in home networks

### WPA2-Enterprise

* Uses authentication server (RADIUS)
* Used in companies and universities

---

# 4. WPA3

WPA3 is the latest Wi-Fi security protocol.

## Features

* Stronger encryption
* Protection against brute-force attacks
* Improved handshake security
* Forward secrecy

---

## WPA3 Authentication: SAE

SAE stands for:

```text id="sae1"
Simultaneous Authentication of Equals
```

Benefits:

* Prevents offline password cracking
* More secure handshake process

---

# WPA vs WPA2 vs WPA3

| Feature                | WPA    | WPA2     | WPA3           |
| ---------------------- | ------ | -------- | -------------- |
| Encryption             | TKIP   | AES      | AES (Stronger) |
| Security Level         | Medium | High     | Very High      |
| Brute Force Protection | Low    | Medium   | High           |
| Status                 | Old    | Standard | Latest         |

---

# Encryption Types in Wi-Fi

## 1. TKIP

* Used in WPA
* Weak compared to AES
* Deprecated

## 2. AES

* Used in WPA2 and WPA3
* Strong encryption
* Industry standard

---

# Key Concepts in Wi-Fi Security

---

## Authentication

Verifying user identity before access.

Example:

```text id="auth1"
Password entry before connecting to Wi-Fi
```

---

## Encryption

Protecting data so it cannot be read by attackers.

Example:

```text id="enc1"
Plain Text → Encrypted Data
```

---

## Integrity

Ensuring data is not modified during transmission.

---

# WPA2 Four-Way Handshake (Basic Idea)

When a device connects:

1. AP sends challenge
2. Client responds
3. Keys are generated
4. Secure connection established

(This will be covered in detail in next file)

---

# Security Comparison with WEP

| Feature    | WEP       | WPA2     | WPA3        |
| ---------- | --------- | -------- | ----------- |
| Security   | Very Weak | Strong   | Very Strong |
| Encryption | RC4       | AES      | AES         |
| Status     | Broken    | Standard | Modern      |

---

# Common Wi-Fi Attacks (Conceptual)

---

## 1. Brute Force Attack

Trying multiple passwords until correct one is found.

---

## 2. Dictionary Attack

Using a list of common passwords.

---

## 3. Packet Capture Attack

Intercepting wireless traffic.

---

## 4. Evil Twin Attack

Fake Access Point pretending to be real Wi-Fi.

---

# WPA Security Best Practices

* Use WPA3 when available
* Prefer WPA2-AES over WPA2-TKIP
* Use strong passwords
* Disable WEP and WPA
* Enable router updates
* Avoid weak passwords like "12345678"

---

# Real-Life Example

Home Wi-Fi:

```text id="home1"
Security: WPA2-Personal
Password: StrongKey@123
Encryption: AES
```

---

# Summary

* WPA, WPA2, and WPA3 are Wi-Fi security protocols.
* WEP is outdated and insecure.
* WPA improved security using TKIP.
* WPA2 uses AES and is widely used.
* WPA3 is the most secure modern standard.
* Strong encryption and authentication are critical for wireless security.
