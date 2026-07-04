# Management Frames

## Description

Management Frames are one of the three primary IEEE 802.11 frame types.

Their purpose is **not to transfer user data**, but to establish, maintain, and terminate communication between wireless devices and Access Points.

Without Management Frames, devices would not be able to discover, join, or leave Wi-Fi networks.

---

# IEEE 802.11 Frame Types

IEEE 802.11 defines three main frame categories:

| Frame Type        | Purpose                           |
| ----------------- | --------------------------------- |
| Management Frames | Manage wireless connections       |
| Control Frames    | Coordinate wireless communication |
| Data Frames       | Carry user data                   |

---

# What are Management Frames?

Management Frames are responsible for:

* Discovering Wi-Fi networks
* Advertising Access Points
* Authenticating devices
* Associating clients
* Maintaining wireless connections
* Ending wireless sessions

---

# Communication Process

A typical Wi-Fi connection starts with Management Frames.

```text id="mf1"
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
Data Transfer
```

---

# Types of Management Frames

The most common Management Frames are:

* Beacon Frame
* Probe Request
* Probe Response
* Authentication
* Deauthentication
* Association Request
* Association Response
* Disassociation

---

# Beacon Frame

A Beacon Frame is periodically transmitted by an Access Point.

Purpose:

* Advertise the wireless network
* Inform nearby devices that the network exists

Information included:

* SSID
* BSSID
* Channel
* Supported data rates
* Security capabilities
* Timestamp

Example:

```text id="beacon1"
Access Point
      │
 Beacon Frame
      │
Nearby Devices
```

---

# Probe Request

A client sends a Probe Request when searching for nearby Wi-Fi networks.

Example:

```text id="probe1"
Laptop
   │
Probe Request
   │
Nearby Access Points
```

Purpose:

* Discover available wireless networks

---

# Probe Response

An Access Point replies with a Probe Response.

Information may include:

* SSID
* Supported rates
* Security information
* Channel

Example:

```text id="probe2"
Access Point
     │
Probe Response
     │
Laptop
```

---

# Authentication Frame

Authentication verifies that a client is allowed to begin the connection process.

Example:

```text id="auth1"
Client
   │
Authentication Request
   │
Access Point
```

Authentication occurs before association.

---

# Association Request

After successful authentication, the client sends an Association Request.

Purpose:

* Request to join the wireless network

Example:

```text id="assoc1"
Client
   │
Association Request
   │
Access Point
```

---

# Association Response

The Access Point replies with an Association Response.

Possible results:

* Accepted
* Rejected

If accepted, the client becomes associated with the Access Point.

---

# Disassociation Frame

Disassociation ends the current association while keeping authentication separate.

Reasons include:

* User disconnects
* Weak signal
* Access Point restart
* Network management

---

# Deauthentication Frame

A Deauthentication Frame ends the authentication relationship.

After deauthentication, the client must authenticate again before reconnecting.

---

# Management Frame Exchange

```text id="flow1"
Access Point                    Station

Beacon ------------------------>

<---------------- Probe Request

Probe Response ---------------->

<-------------- Authentication

Authentication Response ------->
<------------ Association Request

Association Response ---------->
```

---

# Information Carried by Management Frames

Management Frames may contain:

* SSID
* BSSID
* MAC Addresses
* Channel
* Supported Standards
* Security Information
* Capabilities
* Timing Information

---

# Management Frames in Wireshark

Wireshark can display Management Frames such as:

* Beacon
* Probe Request
* Probe Response
* Authentication
* Association
* Deauthentication
* Disassociation

These frames help analyze how devices discover and connect to wireless networks.

---

# Importance in Networking

Management Frames make wireless networking possible by enabling devices to:

* Discover networks
* Join networks
* Maintain connections
* Disconnect properly

Without them, communication cannot begin.

---

# Management Frames in Cybersecurity

Security professionals analyze Management Frames to:

* Troubleshoot wireless issues
* Detect rogue Access Points
* Study roaming behavior
* Verify authentication and association processes
* Investigate wireless connectivity problems

Understanding these frames is an important part of wireless security analysis.

---

# Summary

* Management Frames control the lifecycle of wireless connections.
* They allow devices to discover, authenticate, associate, and disconnect from Wi-Fi networks.
* Common Management Frames include Beacon, Probe Request, Probe Response, Authentication, Association, Disassociation, and Deauthentication.
* They do not carry normal user data.
* Understanding Management Frames is essential for networking, Wireshark analysis, and cybersecurity.
