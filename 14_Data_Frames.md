# Data Frames

## Description

Data Frames are one of the three primary IEEE 802.11 frame types.

Their purpose is to **carry actual user data** between wireless devices and Access Points.

Whenever you browse the web, stream videos, send emails, or transfer files over Wi-Fi, your information is transmitted using Data Frames.

---

# IEEE 802.11 Frame Types

| Frame Type        | Purpose                                   |
| ----------------- | ----------------------------------------- |
| Management Frames | Establish and manage wireless connections |
| Control Frames    | Coordinate wireless communication         |
| Data Frames       | Carry user data                           |

---

# What are Data Frames?

Data Frames transport application data across a Wi-Fi network.

Examples of data carried include:

* Web pages
* Emails
* Chat messages
* Images
* Videos
* Audio streams
* File transfers

Without Data Frames, users would not be able to exchange information over Wi-Fi.

---

# Data Communication Process

```text
Laptop
   │
Data Frame
   │
Access Point
   │
Router
   │
Internet
```

The Data Frame carries user information between devices.

---

# Structure of a Data Frame

A simplified IEEE 802.11 Data Frame contains:

```text
+--------------------------------------+
| MAC Header                           |
+--------------------------------------+
| Frame Control                        |
| Duration                             |
| Address Fields                       |
| Sequence Number                      |
+--------------------------------------+
| Payload (User Data)                  |
+--------------------------------------+
| Frame Check Sequence (FCS)           |
+--------------------------------------+
```

---

# MAC Header

The MAC Header contains information needed for wireless communication.

It typically includes:

* Source MAC Address
* Destination MAC Address
* BSSID
* Frame Control
* Sequence Number

This information helps deliver the frame to the correct destination.

---

# Payload

The Payload contains the actual user information.

Examples:

* HTTP requests
* HTTPS traffic
* DNS queries
* Images
* Documents
* Video packets

The payload is the most important part of a Data Frame because it carries the user's data.

---

# Frame Check Sequence (FCS)

The FCS is used to detect transmission errors.

Purpose:

* Verify frame integrity
* Detect corrupted frames
* Improve communication reliability

If an error is detected, the damaged frame is discarded and may be retransmitted.

---

# Types of Data Frames

IEEE 802.11 defines several Data Frame subtypes.

Common examples include:

* Standard Data Frame
* QoS Data Frame
* Null Data Frame

Each subtype has a specific purpose.

---

# QoS Data Frame

QoS stands for:

```text
Quality of Service
```

QoS Data Frames prioritize important traffic.

Examples:

* Voice calls
* Video conferencing
* Online gaming
* Video streaming

Benefits:

* Lower latency
* Better performance
* Improved user experience

---

# Encrypted Data Frames

Modern Wi-Fi networks encrypt Data Frames to protect user information.

Common security protocols include:

| Protocol | Encryption     |
| -------- | -------------- |
| WPA      | TKIP           |
| WPA2     | AES            |
| WPA3     | AES (Enhanced) |

Encryption helps maintain:

* Confidentiality
* Integrity
* Privacy

---

# Unicast Data

Unicast communication occurs between one sender and one receiver.

Example:

```text
Laptop
   │
Data
   │
Access Point
```

This is the most common type of wireless communication.

---

# Broadcast Data

Broadcast communication sends data to all devices on the network.

Example:

```text
Access Point
   │
 ├── Laptop
 ├── Phone
 ├── Tablet
 └── Smart TV
```

Every connected device receives the frame.

---

# Multicast Data

Multicast communication sends data to a specific group of devices.

Example:

```text
Server
   │
Multicast
   │
Selected Devices Only
```

Not every device receives the frame.

---

# Data Frame Transmission

A simplified communication flow:

```text
Station
   │
Data Frame
   │
Access Point
   │
ACK
   │
Station
```

After receiving the Data Frame successfully, the receiver typically sends an ACK (Acknowledgment).

---

# Data Frames in Wireshark

Wireshark allows you to inspect Data Frames and view information such as:

* Source Address
* Destination Address
* BSSID
* Payload Details (when available)
* Protocol Information
* Frame Length

This helps administrators troubleshoot wireless communication.

---

# Real-Life Example

Suppose you open a website.

The process involves:

```text
Laptop
   │
HTTP/HTTPS Request
   │
Data Frame
   │
Access Point
   │
Router
   │
Internet
```

The website's response is also delivered using Data Frames.

---

# Data Frames in Cybersecurity

Security professionals analyze Data Frames to:

* Troubleshoot network issues
* Understand protocol behavior
* Investigate connectivity problems
* Validate wireless communication
* Study encrypted traffic patterns

In secure networks, the payload is typically encrypted, helping protect user privacy.

---

# Summary

* Data Frames transport user information across Wi-Fi networks.
* They contain a MAC Header, Payload, and Frame Check Sequence (FCS).
* The Payload carries application data such as web traffic, emails, and videos.
* QoS Data Frames improve performance for latency-sensitive applications.
* Modern Wi-Fi networks encrypt Data Frames using protocols such as WPA2 and WPA3.
* Understanding Data Frames is essential for networking, Wireshark analysis, and cybersecurity.
