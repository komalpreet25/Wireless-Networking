# MAC Address in Wi-Fi

## Description

A **MAC (Media Access Control) Address** is a unique hardware identifier assigned to a network interface.

In Wi-Fi networks, MAC addresses help identify wireless devices and enable communication between Stations (STAs) and Access Points (APs).

Unlike IP addresses, which can change, a MAC address is associated with the network interface itself.

---

# What is a MAC Address?

A MAC Address is a **48-bit (6-byte)** hexadecimal identifier assigned to a network interface.

Example:

```text
00:1A:2B:3C:4D:5E
```

Each network interface (Wi-Fi or Ethernet) has its own MAC address.

---

# Why is a MAC Address Important?

A MAC Address is used to:

* Identify network devices
* Deliver frames within a local network
* Support wireless communication
* Distinguish one device from another

Without MAC addresses, devices would not know where to send data within a LAN or WLAN.

---

# MAC Address Format

A MAC address contains six groups of hexadecimal digits.

Example:

```text
AA:BB:CC:DD:EE:FF
```

Each pair represents one byte.

---

# Hexadecimal Values

A MAC Address uses hexadecimal numbers.

Possible characters are:

```text
0 1 2 3 4 5 6 7 8 9 A B C D E F
```

Each character represents 4 bits.

---

# Structure of a MAC Address

A MAC Address has two main parts:

| Part                             | Purpose                 |
| -------------------------------- | ----------------------- |
| OUI (First 24 Bits)              | Manufacturer Identifier |
| Device Identifier (Last 24 Bits) | Unique Device Number    |

Example:

```text
00:1A:2B : 3C:4D:5E
│ OUI │ │ Device ID │
```

---

# OUI (Organizationally Unique Identifier)

OUI stands for:

```text
Organizationally Unique Identifier
```

The OUI identifies the hardware manufacturer.

Examples:

* Intel
* Qualcomm
* Broadcom
* TP-Link
* Cisco

Manufacturers receive OUIs from IEEE.

---

# Device Identifier

The last 24 bits uniquely identify a specific network interface produced by that manufacturer.

This makes each MAC Address unique.

---

# MAC Address vs IP Address

| Feature     | MAC Address           | IP Address               |
| ----------- | --------------------- | ------------------------ |
| Layer       | Data Link (Layer 2)   | Network (Layer 3)        |
| Assigned By | Manufacturer          | Network / DHCP           |
| Changes     | Usually No            | Yes (can change)         |
| Purpose     | Device Identification | Routing Between Networks |

---

# MAC Address in Wi-Fi Communication

Example:

```text
Laptop
MAC:
AA:BB:CC:11:22:33

↓

Access Point

↓

Phone
MAC:
DD:EE:FF:44:55:66
```

Data Frames use MAC addresses to identify the sender and receiver.

---

# Source and Destination MAC Address

Every Data Frame contains:

* Source MAC Address
* Destination MAC Address

Example:

```text
Source:
AA:BB:CC:11:22:33

↓

Destination:
DD:EE:FF:44:55:66
```

---

# BSSID

The BSSID is the MAC Address of the Access Point.

Example:

```text
SSID:
Office_WiFi

BSSID:
A4:6C:2A:89:10:7F
```

Every Access Point has a unique BSSID.

---

# Unicast MAC Address

A Unicast MAC Address identifies one device.

Example:

```text
Laptop
↓

Access Point
```

Communication occurs between one sender and one receiver.

---

# Broadcast MAC Address

The Broadcast MAC Address is:

```text
FF:FF:FF:FF:FF:FF
```

A Broadcast Frame is delivered to every device on the local network.

---

# Multicast MAC Address

A Multicast MAC Address sends data to a selected group of devices.

Example:

```text
Server
↓

Selected Devices Only
```

Not every device receives the frame.

---

# MAC Randomization

Modern smartphones and laptops may use **MAC Randomization** when scanning or joining Wi-Fi networks.

Purpose:

* Improve privacy
* Reduce device tracking
* Hide the device's permanent MAC Address from nearby observers

Many modern operating systems enable this feature by default.

---

# MAC Filtering

Some routers allow administrators to create a list of allowed or blocked MAC addresses.

Example:

```text
Allowed Devices

AA:BB:CC:11:22:33
DD:EE:FF:44:55:66
```

Only listed devices are permitted to connect.

While useful for basic access control, MAC filtering should not be considered a strong security mechanism by itself.

---

# MAC Address in Wireshark

Wireshark displays MAC-related information, including:

* Source Address
* Destination Address
* Receiver Address
* Transmitter Address
* BSSID

This helps analyze wireless communication.

---

# Real-Life Example

Home Wi-Fi:

```text
Router (BSSID)
↓

Laptop
MAC:
AA:BB:CC:11:22:33

↓

Phone
MAC:
DD:EE:FF:44:55:66
```

Each device is uniquely identified by its MAC Address.

---

# MAC Address in Cybersecurity

Security professionals analyze MAC addresses to:

* Identify devices
* Understand wireless communication
* Investigate network incidents
* Detect duplicate addresses
* Troubleshoot connectivity issues

MAC addresses are an important part of wireless packet analysis.

---

# Summary

* A MAC Address uniquely identifies a network interface.
* It is a 48-bit hexadecimal address.
* The first 24 bits are the OUI (manufacturer identifier).
* The last 24 bits uniquely identify the device.
* Data Frames use Source and Destination MAC Addresses.
* The BSSID is the MAC Address of an Access Point.
* MAC Randomization improves user privacy.
* MAC Filtering provides basic access control but is not a replacement for strong Wi-Fi security.
* Understanding MAC addresses is fundamental for networking, Wireshark analysis, and cybersecurity.
