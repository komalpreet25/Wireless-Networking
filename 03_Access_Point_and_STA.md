# Access Point (AP) and Station (STA)

## Description

An Access Point (AP) and a Station (STA) are the two primary components of a Wi-Fi network.

The Access Point provides wireless connectivity, while Stations are the client devices that connect to the wireless network.

Understanding AP and STA is essential before learning wireless authentication, packet capture, monitor mode, and wireless security.

---

# What is an Access Point (AP)?

An **Access Point (AP)** is a networking device that allows wireless devices to connect to a wired network.

It broadcasts the Wi-Fi network and manages communication with connected clients.

Examples:

* Home Wi-Fi Router
* Enterprise Access Point
* Office Wireless Router

---

# Functions of an Access Point

An AP performs several important tasks:

* Broadcasts the Wi-Fi network (SSID)
* Authenticates wireless clients
* Associates client devices
* Transmits and receives wireless frames
* Manages connected devices
* Bridges wireless and wired networks

---

# Access Point Diagram

```text
             Internet
                 │
              Modem
                 │
              Router
                 │
          Access Point
          /     |      \
      Laptop  Phone   Tablet
```

The Access Point allows wireless devices to communicate with the network.

---

# What is a Station (STA)?

A **Station (STA)** is any wireless device that supports the IEEE 802.11 standard.

A Station communicates with an Access Point to access the network.

Examples:

* Laptop
* Smartphone
* Tablet
* Smart TV
* Printer
* IoT Device

---

# Station Functions

A Station can:

* Discover Wi-Fi networks
* Authenticate with an AP
* Associate with an AP
* Send and receive data
* Disconnect from the network

---

# AP and STA Communication

Communication begins after a Station joins the network.

```text
Station
   │
Authentication
   │
Association
   │
Data Communication
   │
Access Point
```

---

# Infrastructure Mode

Infrastructure Mode is the most common Wi-Fi mode.

All wireless devices communicate through an Access Point.

```text
 Laptop
    │
 Phone ── Access Point ── Internet
    │
Tablet
```

Advantages:

* Easy management
* Internet connectivity
* Better security
* Supports many devices

---

# Ad Hoc Mode

In Ad Hoc Mode, devices communicate directly with each other.

No Access Point is required.

```text
Laptop  ─────────  Laptop
```

Advantages:

* No router required
* Simple setup

Disadvantages:

* Limited range
* Limited scalability
* Rarely used today

---

# Difference Between Infrastructure and Ad Hoc Mode

| Feature               | Infrastructure  | Ad Hoc                |
| --------------------- | --------------- | --------------------- |
| Access Point Required | Yes             | No                    |
| Internet Access       | Yes             | Usually No            |
| Scalability           | High            | Low                   |
| Management            | Easy            | Difficult             |
| Common Usage          | Homes & Offices | Temporary Connections |

---

# Authentication

Before joining a Wi-Fi network, the Station must authenticate.

Authentication verifies the identity of the client.

Example:

```text
Station
    │
Authentication Request
    │
Access Point
```

---

# Association

After authentication, the Station associates with the Access Point.

Association creates an active wireless connection.

```text
Authentication
      ↓
Association
      ↓
Connected
```

---

# Disassociation

When a device leaves the network, it becomes disassociated.

Reasons include:

* User disconnects
* Signal loss
* AP restart
* Timeout

---

# Roaming

Roaming allows a Station to move between Access Points without manually reconnecting.

Example:

```text
AP 1  ───────►  AP 2
```

The device automatically connects to the stronger Access Point.

---

# BSS (Basic Service Set)

A BSS consists of:

* One Access Point
* One or more Stations

```text
      AP
    / | \
 STA STA STA
```

Each BSS has a unique identifier called the **BSSID**.

---

# ESS (Extended Service Set)

An ESS consists of multiple Access Points connected together.

They usually share the same SSID.

```text
      AP1 -------- AP2 -------- AP3
       │            │            │
     Clients      Clients      Clients
```

Benefits:

* Larger wireless coverage
* Seamless roaming
* Better scalability

---

# AP Responsibilities

An Access Point is responsible for:

* Broadcasting beacon frames
* Handling authentication
* Managing associations
* Forwarding traffic
* Supporting roaming

---

# STA Responsibilities

A Station is responsible for:

* Scanning for networks
* Sending authentication requests
* Associating with an AP
* Exchanging wireless frames
* Disconnecting when needed

---

# AP vs STA

| Feature          | Access Point   | Station       |
| ---------------- | -------------- | ------------- |
| Device Type      | Network Device | Client Device |
| Broadcasts Wi-Fi | Yes            | No            |
| Connects Clients | Yes            | No            |
| Uses SSID        | Broadcasts     | Connects      |
| Examples         | Router, AP     | Laptop, Phone |

---

# Real-Life Example

At home:

```text
ISP
 │
Modem
 │
Wi-Fi Router (AP)
 │
 ├── Laptop (STA)
 ├── Phone (STA)
 ├── TV (STA)
 └── Tablet (STA)
```

All client devices communicate through the Access Point.

---

# AP and STA in Cybersecurity

Security professionals analyze APs and STAs to:

* Monitor wireless traffic
* Detect unauthorized devices
* Investigate rogue access points
* Capture wireless frames
* Troubleshoot wireless issues

Understanding AP and STA behavior is essential before learning:

* Four-Way Handshake
* Monitor Mode
* Packet Injection
* Wireless Packet Analysis

---

# Summary

* An Access Point (AP) provides wireless connectivity.
* A Station (STA) is any wireless client device.
* Infrastructure Mode is the most common Wi-Fi deployment.
* Ad Hoc Mode allows direct device-to-device communication.
* Authentication occurs before Association.
* BSS contains one AP and connected STAs.
* ESS combines multiple APs for larger coverage.
* Understanding AP and STA is fundamental for wireless networking and cybersecurity.
