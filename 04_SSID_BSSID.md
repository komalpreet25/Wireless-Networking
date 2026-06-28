# SSID and BSSID

## Description

SSID and BSSID are two fundamental identifiers used in Wi-Fi networks.

* **SSID** identifies the wireless network by its name.
* **BSSID** uniquely identifies a specific Access Point using its MAC address.

Understanding these concepts is essential for wireless networking, Wireshark analysis, monitor mode, and wireless security.

---

# What is SSID?

SSID stands for:

```text id="ssid1"
Service Set Identifier
```

The SSID is the **name of a Wi-Fi network** that users see when searching for available wireless networks.

Examples:

* Home_WiFi
* Office_Network
* CoffeeShop_WiFi
* MyRouter

---

# Purpose of SSID

The SSID helps users:

* Identify a wireless network
* Connect to the correct network
* Differentiate between multiple Wi-Fi networks

---

# Example

Your phone may display:

```text id="ssid2"
Available Networks

Home_WiFi
Office_WiFi
Library
CoffeeShop
```

Each name shown is an SSID.

---

# What is BSSID?

BSSID stands for:

```text id="bssid1"
Basic Service Set Identifier
```

A BSSID is the **MAC address of an Access Point**.

Unlike the SSID, which is a readable network name, the BSSID is a unique hardware identifier.

Example:

```text id="bssid2"
34:AB:56:91:CD:EF
```

Every Access Point has its own BSSID.

---

# Why is BSSID Important?

The BSSID helps devices:

* Identify a specific Access Point
* Distinguish between multiple APs using the same SSID
* Support roaming in larger wireless networks

---

# SSID vs BSSID

| Feature          | SSID         | BSSID                    |
| ---------------- | ------------ | ------------------------ |
| Meaning          | Network Name | Access Point MAC Address |
| Visible to Users | Yes          | Usually No               |
| Unique           | Not Always   | Yes                      |
| Example          | Home_WiFi    | 34:AB:56:91:CD:EF        |

---

# Relationship Between SSID and BSSID

A single SSID can have multiple BSSIDs.

Example:

```text id="rel1"
SSID: Office_WiFi

AP1 → AA:AA:AA:AA:AA:01

AP2 → AA:AA:AA:AA:AA:02

AP3 → AA:AA:AA:AA:AA:03
```

All three Access Points broadcast the same SSID but have different BSSIDs.

---

# What is ESSID?

ESSID stands for:

```text id="essid1"
Extended Service Set Identifier
```

In modern networking, **ESSID and SSID are commonly treated as the same thing**.

The ESSID allows multiple Access Points to share the same network name.

---

# Hidden SSID

A network administrator can configure an Access Point to stop broadcasting its SSID.

This is called a **Hidden SSID**.

Example:

```text id="hidden1"
Available Networks

Home_WiFi
Office_WiFi
Hidden Network
CoffeeShop
```

The network still exists but does not broadcast its name in beacon frames.

---

# Is a Hidden SSID Secure?

No.

A hidden SSID is **not** a strong security measure.

The SSID can often be discovered during normal wireless communication between authorized devices and the Access Point.

---

# Beacon Frames

Access Points periodically send **Beacon Frames**.

These frames contain information such as:

* SSID
* Supported data rates
* Channel
* Security capabilities
* BSSID

Beacon frames help nearby devices discover wireless networks.

---

# Probe Request

A Station sends a **Probe Request** to search for nearby Wi-Fi networks.

Example:

```text id="probe1"
Laptop
   │
Probe Request
   │
Nearby Access Points
```

---

# Probe Response

An Access Point replies with a **Probe Response** containing information about the network.

Example:

```text id="probe2"
Access Point
     │
Probe Response
     │
Laptop
```

---

# Multiple SSIDs

One Access Point can broadcast multiple SSIDs.

Example:

```text id="multi1"
Home_WiFi
Guest_WiFi
Office_WiFi
```

Each SSID may have different security settings and access permissions.

---

# SSID Naming Best Practices

Good practices include:

* Use meaningful names
* Avoid personal information
* Avoid default router names
* Keep names easy to recognize

Example:

```text id="goodssid"
Office_WiFi
```

Avoid names like:

```text id="badssid"
John_House_123
```

---

# BSSID Example

A Wi-Fi analyzer may display:

```text id="bssid3"
SSID : Home_WiFi

BSSID :
34:AB:56:91:CD:EF
```

The SSID identifies the network, while the BSSID identifies the Access Point.

---

# SSID and BSSID in Wireshark

During wireless packet analysis, you may observe:

* SSID
* BSSID
* Source MAC Address
* Destination MAC Address
* Beacon Frames
* Probe Requests
* Probe Responses

These details help analyze wireless communication.

---

# Real-Life Example

A university campus may have:

```text id="campus"
SSID:
University_WiFi

Building A
BSSID:
00:11:22:33:44:01

Building B
BSSID:
00:11:22:33:44:02

Building C
BSSID:
00:11:22:33:44:03
```

Students see only **University_WiFi**, while their devices connect to the nearest Access Point based on its BSSID.

---

# SSID and Cybersecurity

Security professionals use SSID and BSSID information to:

* Identify wireless networks
* Detect rogue Access Points
* Analyze wireless traffic
* Troubleshoot Wi-Fi issues
* Investigate wireless environments

---

# Summary

* SSID is the name of a Wi-Fi network.
* BSSID is the MAC address of an Access Point.
* Multiple Access Points can share the same SSID while using different BSSIDs.
* Beacon Frames advertise wireless networks.
* Probe Requests and Probe Responses help devices discover Wi-Fi networks.
* Hidden SSIDs do not provide strong security.
* Understanding SSID and BSSID is essential for wireless networking, Wireshark, and cybersecurity.
