# WIDS and WIPS

## Description

WIDS (Wireless Intrusion Detection System) and WIPS (Wireless Intrusion Prevention System) are wireless security technologies used to monitor, detect, and respond to unauthorized or suspicious wireless activity.

They help organizations protect Wi-Fi networks from Rogue Access Points, Evil Twin networks, unauthorized devices, and wireless security threats.

---

# What is WIDS?

WIDS stands for:

```text id="wids1"
Wireless Intrusion Detection System
```

A WIDS continuously monitors wireless activity and alerts administrators when suspicious behavior is detected.

Its primary purpose is:

* Detection
* Monitoring
* Alerting

A WIDS does not automatically block threats.

---

# What is WIPS?

WIPS stands for:

```text id="wips1"
Wireless Intrusion Prevention System
```

A WIPS not only detects suspicious activity but can also take actions to prevent or contain threats.

Its primary purpose is:

* Detection
* Monitoring
* Prevention
* Response

---

# WIDS vs WIPS

| Feature            | WIDS | WIPS |
| ------------------ | ---- | ---- |
| Detect Threats     | Yes  | Yes  |
| Generate Alerts    | Yes  | Yes  |
| Prevent Threats    | No   | Yes  |
| Automated Response | No   | Yes  |

---

# Why Are WIDS and WIPS Important?

Wireless networks are constantly exposed to:

* Unauthorized devices
* Rogue Access Points
* Evil Twin networks
* Policy violations
* Misconfigured wireless equipment

WIDS and WIPS improve visibility and security.

---

# How WIDS Works

A WIDS continuously listens to wireless traffic.

Example:

```text id="wids2"
Wireless Network
        │
WIDS Sensor
        │
Monitor Activity
        │
Generate Alerts
```

When suspicious activity is detected, administrators are notified.

---

# How WIPS Works

A WIPS performs monitoring and prevention.

Example:

```text id="wips2"
Wireless Network
        │
WIPS Sensor
        │
Detect Threat
        │
Take Response Action
```

This helps reduce exposure to wireless threats.

---

# Common Wireless Threats

WIDS and WIPS may detect:

* Rogue Access Points
* Evil Twin Networks
* Unauthorized Clients
* Unknown SSIDs
* Policy Violations
* Misconfigured Access Points

---

# Rogue Access Point Detection

Example:

```text id="rogue1"
Approved APs:
AP1
AP2
AP3

Detected:
Unknown AP
```

The system identifies devices that are not part of the approved inventory.

---

# Evil Twin Detection

Example:

```text id="evil1"
Legitimate SSID:
Office_WiFi

Suspicious SSID:
Office_WiFi
```

Duplicate or suspicious wireless networks may trigger alerts.

---

# Wireless Sensors

WIDS/WIPS solutions often use sensors.

Purpose:

* Monitor wireless traffic
* Observe radio activity
* Detect suspicious events

Sensors may be dedicated devices or integrated into Access Points.

---

# Monitoring Activities

A WIDS/WIPS can monitor:

* SSIDs
* BSSIDs
* Beacon Frames
* Probe Requests
* Authentication Events
* Association Events

This provides visibility into wireless environments.

---

# Alerting

When suspicious activity is detected:

```text id="alert1"
Threat Detected
      │
Alert Generated
      │
Administrator Notified
```

This allows security teams to investigate quickly.

---

# Prevention Capabilities

Unlike WIDS, a WIPS can take defensive actions.

Examples include:

* Containment policies
* Device isolation
* Access restrictions
* Automated responses

The exact response depends on organizational policies.

---

# Enterprise Wireless Security

Large organizations often deploy:

* Centralized wireless management
* WIDS
* WIPS
* Security monitoring platforms

These technologies improve wireless visibility and control.

---

# Benefits of WIDS/WIPS

Benefits include:

* Improved wireless visibility
* Faster threat detection
* Better policy enforcement
* Reduced security risks
* Continuous monitoring

---

# Example Workflow

```text id="flow1"
Monitor Wireless Activity
          ↓
Detect Suspicious Event
          ↓
Generate Alert
          ↓
Investigate
          ↓
Respond
```

For WIPS:

```text id="flow2"
Monitor
   ↓
Detect
   ↓
Prevent
   ↓
Report
```

---

# WIDS/WIPS and Site Surveys

WIDS/WIPS complements Wireless Site Surveys by:

* Continuously monitoring networks
* Detecting changes over time
* Identifying new devices
* Discovering unauthorized activity

---

# WIDS/WIPS in Cybersecurity

Cybersecurity professionals use WIDS/WIPS to:

* Detect Rogue APs
* Identify Evil Twins
* Enforce wireless policies
* Improve wireless security posture
* Investigate wireless incidents

These technologies are important components of enterprise wireless defense.

---

# Real-Life Example

A company maintains an inventory of approved Access Points.

One day, a new wireless network appears with an unknown BSSID.

The WIDS detects the device and generates an alert.

The security team investigates and discovers an unauthorized Access Point connected to the corporate network.

---

# Summary

* WIDS monitors wireless activity and detects suspicious behavior.
* WIPS provides detection plus prevention capabilities.
* Both technologies improve wireless security visibility.
* They help identify Rogue Access Points, Evil Twins, and unauthorized devices.
* WIDS focuses on detection and alerting.
* WIPS focuses on detection, alerting, and response.
* WIDS and WIPS are important components of enterprise wireless security.
