# Evil Twin Attack

## Description

An Evil Twin is a fraudulent wireless Access Point that impersonates a legitimate Wi-Fi network.

It is designed to appear identical or very similar to a trusted wireless network so that users mistakenly connect to it.

Evil Twin attacks are important to understand because they demonstrate how trust in wireless network names (SSIDs) alone can be dangerous.

---

# What is an Evil Twin?

An Evil Twin is a wireless network that imitates a legitimate Wi-Fi network.

Example:

```text id="evil1"
Legitimate Network:
CoffeeShop_WiFi

Fake Network:
CoffeeShop_WiFi
```

To a user, both networks may appear identical.

---

# Why is it Called an Evil Twin?

The term "twin" is used because the fake network attempts to look like the legitimate one.

Example:

```text id="twin1"
Real AP
   │
CoffeeShop_WiFi

Fake AP
   │
CoffeeShop_WiFi
```

Both appear similar, making it difficult for users to distinguish between them.

---

# How Users Get Confused

Many users identify Wi-Fi networks only by their SSID.

However:

```text id="ssid1"
SSID ≠ Identity
```

Different Access Points can broadcast the same SSID.

Because of this, users may unknowingly connect to an untrusted network.

---

# Evil Twin vs Rogue Access Point

These terms are related but different.

## Rogue Access Point

* Unauthorized Access Point
* May be accidental
* Does not need to imitate another network

---

## Evil Twin

* Intentionally imitates a legitimate network
* Uses a similar or identical SSID
* Attempts to appear trustworthy

---

# Comparison

| Feature                   | Rogue AP        | Evil Twin |
| ------------------------- | --------------- | --------- |
| Unauthorized              | Yes             | Yes       |
| May Be Accidental         | Yes             | No        |
| Mimics Legitimate Network | No              | Yes       |
| Designed to Mislead Users | Not Necessarily | Yes       |

---

# Why Evil Twins Are a Risk

Users may trust the network because:

* The SSID looks familiar
* The network appears legitimate
* They have connected to a similarly named network before

This demonstrates why users should not rely solely on SSID names.

---

# Legitimate Network Identification

Access Points are uniquely identified by their:

```text id="bssid1"
BSSID
```

The BSSID is the MAC Address of the Access Point.

Example:

```text id="bssid2"
SSID:
Office_WiFi

BSSID:
A4:6C:2A:89:10:7F
```

Different Access Points may share an SSID, but their BSSIDs are different.

---

# Signs of a Suspicious Wireless Network

Possible warning signs include:

* Unexpected duplicate SSIDs
* Unknown BSSIDs
* Unusual signal strength
* Security settings different from expected
* Unexpected login prompts

These signs do not prove an Evil Twin exists, but they may justify further investigation.

---

# Detection Methods

Organizations use:

* Wireless monitoring systems
* Wireless intrusion detection systems (WIDS)
* Site surveys
* Access Point inventories
* BSSID verification

These methods help identify unauthorized wireless networks.

---

# Importance of Wireless Monitoring

Monitoring helps administrators:

* Identify unknown Access Points
* Compare observed BSSIDs with approved inventories
* Investigate suspicious wireless activity

---

# Wireless Site Survey

A site survey can reveal:

* Duplicate SSIDs
* Unknown Access Points
* Coverage anomalies
* Unexpected wireless devices

---

# User Awareness

Users should:

* Verify the correct network name
* Confirm security settings
* Be cautious of duplicate SSIDs
* Follow organizational wireless policies

Awareness is one of the strongest defenses against deceptive wireless networks.

---

# Enterprise Security Controls

Organizations often deploy:

* WPA2-Enterprise or WPA3-Enterprise
* Certificate-based authentication
* WIDS/WIPS solutions
* Centralized wireless management

These controls help strengthen wireless security.

---

# Evil Twin and Wireshark

Wireless analysis tools can help identify:

* Beacon Frames
* Probe Responses
* SSIDs
* BSSIDs
* Security capabilities

This information assists administrators in understanding wireless environments.

---

# Real-Life Example

Imagine a company named Example Corp.

Employees normally connect to:

```text id="real1"
ExampleCorp_WiFi
```

A second network appears with the same SSID but a different BSSID.

Network administrators investigate because duplicate SSIDs may indicate a configuration issue or an unauthorized device.

---

# Evil Twin in Cybersecurity

Cybersecurity professionals study Evil Twin attacks to:

* Understand wireless trust relationships
* Improve wireless security awareness
* Detect unauthorized wireless devices
* Strengthen network monitoring practices

Knowledge of Evil Twins helps organizations reduce wireless security risks.

---

# Summary

* An Evil Twin is a wireless network that imitates a legitimate Wi-Fi network.
* It typically uses a similar or identical SSID.
* SSIDs alone should not be trusted as proof of identity.
* BSSIDs uniquely identify Access Points.
* Organizations detect suspicious wireless activity using monitoring, inventories, and site surveys.
* Understanding Evil Twins is important for wireless security awareness and cybersecurity.
