# Wireshark for Wireless Analysis

## Description

Wireshark is a powerful open-source network protocol analyzer used to capture, inspect, and analyze network traffic.

In wireless networking, Wireshark helps security professionals, network engineers, and students understand how Wi-Fi devices communicate using the IEEE 802.11 protocol.

It is widely used for troubleshooting, protocol analysis, and learning wireless networking concepts.

---

# What is Wireshark?

Wireshark is a packet analyzer that captures network traffic and displays each packet in a human-readable format.

It allows users to inspect protocols, packet details, timing information, and communication between devices.

---

# Why Use Wireshark?

Wireshark helps you:

* Capture network packets
* Analyze Wi-Fi communication
* Troubleshoot network issues
* Study network protocols
* Identify connection problems
* Learn packet structures

---

# Packet Capture Process

A simplified workflow:

```text id="capture1"
Network Traffic
      │
Wireshark
      │
Packet Capture
      │
Packet Analysis
```

---

# Wireshark and Wireless Networks

When used with a compatible wireless adapter (and supported operating system), Wireshark can capture IEEE 802.11 wireless frames.

This allows you to observe how wireless devices communicate.

---

# IEEE 802.11 Frames in Wireshark

Common wireless frame types include:

* Management Frames
* Control Frames
* Data Frames

Each frame type serves a different purpose in Wi-Fi communication.

---

# Common Management Frames

Examples:

* Beacon Frame
* Probe Request
* Probe Response
* Authentication
* Association Request
* Association Response

These frames help establish and manage wireless connections.

---

# Control Frames

Control Frames help manage wireless communication.

Examples include:

* ACK (Acknowledgment)
* RTS (Request to Send)
* CTS (Clear to Send)

---

# Data Frames

Data Frames carry user information.

Examples:

* Web browsing traffic
* Email data
* File transfers
* Video streaming packets

---

# Packet Details

Each captured packet contains useful information, such as:

* Source MAC Address
* Destination MAC Address
* BSSID
* SSID (when applicable)
* Channel Information
* Signal Details
* Protocol Information

---

# Example Packet Structure

```text id="packet1"
Frame Number
Time
Source
Destination
Protocol
Packet Length
Packet Details
```

---

# Display Filters

Wireshark uses **display filters** to help analyze specific traffic.

Common examples:

| Filter  | Purpose                             |
| ------- | ----------------------------------- |
| `wlan`  | Show all IEEE 802.11 packets        |
| `eapol` | Show authentication (EAPOL) packets |
| `arp`   | Show ARP packets                    |
| `icmp`  | Show ICMP packets                   |
| `dns`   | Show DNS packets                    |
| `tcp`   | Show TCP packets                    |
| `udp`   | Show UDP packets                    |

---

# Wireless Connection Process

A typical Wi-Fi connection includes:

```text id="connect1"
Beacon
    ↓
Probe Request
    ↓
Probe Response
    ↓
Authentication
    ↓
Association
    ↓
Four-Way Handshake
    ↓
Secure Communication
```

Wireshark allows you to observe each step of this process.

---

# Finding Devices

Wireshark helps identify:

* Access Points
* Client Devices (Stations)
* MAC Addresses
* Wireless Channels
* Signal Information

This is useful for troubleshooting and understanding network topology.

---

# Packet Analysis Workflow

```text id="workflow1"
Capture Packets
      │
Apply Filters
      │
Inspect Frames
      │
Analyze Communication
      │
Identify Network Issues
```

---

# Common Use Cases

Network administrators use Wireshark to:

* Diagnose connectivity issues
* Analyze wireless performance
* Verify protocol behavior
* Investigate packet loss
* Study wireless communication

---

# Advantages

* Free and open source
* Supports hundreds of protocols
* Powerful filtering
* Detailed packet inspection
* Cross-platform support
* Excellent learning tool

---

# Limitations

* Requires compatible hardware for wireless capture
* Large captures can be difficult to analyze
* Packet analysis requires networking knowledge
* Some wireless information depends on adapter capabilities

---

# Wireshark and Cybersecurity

Cybersecurity professionals use Wireshark to:

* Analyze network traffic
* Investigate security incidents
* Troubleshoot authentication issues
* Understand protocol behavior
* Validate network configurations

Wireshark is primarily an **analysis tool**. It captures and displays traffic rather than modifying it.

---

# Summary

* Wireshark is a powerful packet analysis tool.
* It captures and displays network traffic in detail.
* It supports analysis of IEEE 802.11 wireless frames.
* Display filters help focus on specific protocols.
* Wireshark is widely used for troubleshooting, learning, and cybersecurity investigations.
* Understanding Wireshark is an essential skill for networking and cybersecurity professionals.
