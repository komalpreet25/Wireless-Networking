# Deauthentication

## Description

Deauthentication is a process in IEEE 802.11 wireless networks that terminates the authentication relationship between a wireless client and an Access Point (AP).

When a device is deauthenticated, it is disconnected from the Wi-Fi network and must authenticate again before reconnecting.

Deauthentication is implemented using a special **Management Frame** known as the Deauthentication Frame.

---

# What is Deauthentication?

Deauthentication is a notification indicating that the authentication relationship between a client and an Access Point has ended.

Example:

```text id="deauth1"
Client
   │
Connected
   │
Access Point

↓

Deauthentication

↓

Client Disconnected
```

After deauthentication, communication stops until the client reconnects.

---

# Authentication vs Deauthentication

| Process          | Purpose                               |
| ---------------- | ------------------------------------- |
| Authentication   | Establish trust between client and AP |
| Deauthentication | End the authentication relationship   |

Authentication starts communication.

Deauthentication ends communication.

---

# IEEE 802.11 Management Frame

Deauthentication is performed using a **Management Frame**.

It is one of the standard frame types defined by IEEE 802.11.

Purpose:

* Notify a device that authentication has ended
* Force reauthentication before reconnection

---

# Connection Lifecycle

A simplified wireless connection process:

```text id="life1"
Authentication
      ↓
Association
      ↓
Data Transfer
      ↓
Deauthentication
      ↓
Disconnected
```

---

# Why Does Deauthentication Occur?

Deauthentication can happen for many legitimate reasons.

Examples:

* User manually disconnects
* Router restarts
* Network maintenance
* Authentication timeout
* Device roaming
* Configuration changes
* Signal issues

---

# Example: User Disconnects

```text id="example1"
Phone
   │
Disconnect Wi-Fi
   │
Access Point
```

The connection is terminated and authentication ends.

---

# Example: Access Point Restart

```text id="example2"
Access Point Restart
        │
Connected Clients
        │
Disconnected
```

Clients must reconnect after the AP becomes available again.

---

# Deauthentication Frame Contents

A Deauthentication Frame typically contains:

* Source Address
* Destination Address
* BSSID
* Reason Code

The Reason Code explains why the connection ended.

---

# Reason Codes

Common examples include:

| Reason                 | Meaning                      |
| ---------------------- | ---------------------------- |
| User Request           | Device disconnected normally |
| AP Shutdown            | Access Point unavailable     |
| Authentication Expired | Session timeout              |
| Roaming Event          | Client moved to another AP   |

---

# Deauthentication vs Disassociation

These terms are often confused.

## Disassociation

* Ends the association
* Authentication may still exist

---

## Deauthentication

* Ends authentication completely
* Reauthentication is required

---

# Comparison

| Feature                   | Disassociation | Deauthentication |
| ------------------------- | -------------- | ---------------- |
| Ends Association          | Yes            | Yes              |
| Ends Authentication       | No             | Yes              |
| Requires Reauthentication | No             | Yes              |

---

# Deauthentication in Wireshark

Wireshark can display Deauthentication Frames.

Useful fields include:

* Source MAC Address
* Destination MAC Address
* BSSID
* Reason Code

Example display:

```text id="wireshark1"
802.11 Deauthentication
Reason Code: Leaving Network
```

---

# Protected Management Frames (PMF)

One weakness of traditional management frames was that they were not always protected.

To improve security, IEEE introduced:

```text id="pmf1"
802.11w
Protected Management Frames (PMF)
```

Purpose:

* Protect important management frames
* Improve wireless security
* Reduce spoofing risks

PMF is commonly used with modern WPA2 and WPA3 deployments.

---

# Why PMF is Important

Protected Management Frames help ensure that critical management communications are authenticated and protected.

Benefits:

* Improved reliability
* Better security
* Protection of management traffic

---

# Deauthentication in Enterprise Networks

Enterprise wireless networks may use:

* WPA2-Enterprise
* WPA3-Enterprise
* PMF
* Centralized wireless management

These features improve the handling and security of management frames.

---

# Real-Life Example

A user walks away from one Access Point and moves closer to another.

Example:

```text id="roaming1"
AP 1
  │
Client
  │
Moving
  ↓
AP 2
```

The client may disconnect from the first AP and establish a connection with the second AP.

---

# Deauthentication in Cybersecurity

Security professionals analyze Deauthentication Frames to:

* Troubleshoot Wi-Fi disconnections
* Investigate roaming behavior
* Diagnose connectivity issues
* Verify wireless configurations
* Study IEEE 802.11 management traffic

Understanding Deauthentication is an important part of wireless network analysis.

---

# Summary

* Deauthentication ends the authentication relationship between a client and an Access Point.
* It is performed using an IEEE 802.11 Management Frame.
* Common causes include user disconnects, AP restarts, roaming, and network maintenance.
* Deauthentication differs from Disassociation because it requires reauthentication.
* Wireshark can display Deauthentication Frames and their reason codes.
* Protected Management Frames (802.11w) improve the security of wireless management traffic.
* Understanding Deauthentication is important for networking, Wireshark analysis, and cybersecurity.
