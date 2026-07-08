# Rogue Access Point

## Description

A Rogue Access Point (Rogue AP) is a wireless Access Point that operates on a network **without proper authorization from the network owner or administrator**.

Rogue Access Points can create security risks because they may allow unauthorized access, bypass security policies, or expose network traffic.

Understanding Rogue APs is important for network administrators and cybersecurity professionals responsible for protecting wireless environments.

---

# What is a Rogue Access Point?

A Rogue Access Point is any wireless Access Point connected to a network without approval.

Example:

```text id="rogue1"
Company Network
      │
Authorized AP
      │
Employees

      │
Unauthorized AP
      │
Rogue Access Point
```

The unauthorized AP may be installed intentionally or accidentally.

---

# How Rogue APs Appear

Common situations include:

* An employee installs a personal Wi-Fi router.
* An unauthorized device is connected to the network.
* A wireless hotspot is improperly connected to internal resources.
* Network policies are ignored.

---

# Why Rogue APs are Dangerous

Rogue Access Points can:

* Bypass security controls
* Create unauthorized wireless access
* Increase the attack surface
* Cause network misconfigurations
* Expose sensitive traffic

Because they are not managed by administrators, they may not follow organizational security standards.

---

# Authorized vs Rogue Access Point

| Feature                   | Authorized AP | Rogue AP       |
| ------------------------- | ------------- | -------------- |
| Approved by Administrator | Yes           | No             |
| Managed by IT Team        | Yes           | Usually No     |
| Follows Security Policies | Yes           | Not Guaranteed |
| Security Risk             | Lower         | Higher         |

---

# Example Scenario

A company has secure wireless infrastructure.

An employee connects a personal router to an office Ethernet port.

Example:

```text id="example1"
Corporate Network
        │
Ethernet Port
        │
Personal Router
        │
Unauthorized Wi-Fi
```

This personal router becomes a Rogue Access Point.

---

# Rogue AP vs Evil Twin

These terms are often confused.

## Rogue Access Point

* Unauthorized Access Point
* Connected to a network without approval
* May not be malicious

---

## Evil Twin

* Designed to imitate a legitimate Wi-Fi network
* Attempts to attract users to connect
* Often used for deceptive purposes

---

# Comparison

| Feature                 | Rogue AP     | Evil Twin  |
| ----------------------- | ------------ | ---------- |
| Unauthorized            | Yes          | Yes        |
| Mimics Legitimate Wi-Fi | Not Required | Yes        |
| May Be Accidental       | Yes          | Usually No |
| Security Risk           | Yes          | Yes        |

---

# Signs of a Rogue Access Point

Possible indicators include:

* Unknown Wi-Fi networks inside the organization
* Unrecognized BSSIDs
* Unexpected wireless coverage
* Unauthorized hardware
* Security policy violations

---

# Detection Methods

Organizations use various methods to identify Rogue APs.

Examples:

* Wireless surveys
* Inventory comparisons
* Wireless monitoring systems
* Network access control systems
* Wi-Fi analysis tools

---

# Wireless Site Survey

A wireless survey helps identify:

* Access Point locations
* SSIDs
* BSSIDs
* Signal coverage
* Unauthorized wireless devices

---

# Importance of BSSID

Each Access Point has a unique BSSID.

Example:

```text id="bssid1"
SSID:
Office_WiFi

BSSID:
A4:6C:2A:89:10:7F
```

Administrators can compare observed BSSIDs with approved device inventories.

---

# Risks of Rogue Access Points

Potential risks include:

* Unauthorized network access
* Security policy violations
* Weak security settings
* Network instability
* Increased attack surface

---

# Prevention Methods

Organizations can reduce risk by:

* Maintaining wireless inventories
* Conducting regular audits
* Monitoring wireless activity
* Enforcing security policies
* Training employees
* Restricting unauthorized devices

---

# Enterprise Wireless Security

Large organizations often implement:

* Wireless intrusion detection systems
* Wireless intrusion prevention systems
* Centralized Access Point management
* Security monitoring solutions

These help identify unauthorized wireless devices quickly.

---

# Rogue AP in Wireshark

Wireshark can help analyze wireless traffic and identify:

* Unknown SSIDs
* Unknown BSSIDs
* Beacon Frames
* Probe Responses

This information assists in wireless investigations.

---

# Real-Life Example

A company's IT department approves five Access Points.

During a wireless survey, a sixth Access Point is discovered.

Investigation reveals that an employee installed a personal wireless router for convenience.

The device is classified as a Rogue Access Point because it was not approved by the organization.

---

# Rogue Access Points in Cybersecurity

Security professionals analyze Rogue APs to:

* Protect corporate networks
* Enforce security policies
* Reduce unauthorized access
* Improve wireless visibility
* Strengthen network security

Understanding Rogue APs is a key part of wireless security management.

---

# Summary

* A Rogue Access Point is an unauthorized wireless Access Point.
* It may create security risks and bypass network policies.
* Rogue APs differ from Evil Twins because they do not necessarily imitate legitimate networks.
* Organizations detect Rogue APs using monitoring, inventories, and wireless surveys.
* Proper wireless security management helps reduce the risks associated with unauthorized Access Points.
* Understanding Rogue APs is important for networking, enterprise security, and cybersecurity.
