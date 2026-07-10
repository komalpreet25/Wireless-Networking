# Wireless Site Survey

## Description

A Wireless Site Survey is the process of analyzing a physical area to understand Wi-Fi coverage, signal strength, interference, channel usage, and Access Point placement.

Site surveys help network administrators design, deploy, troubleshoot, and optimize wireless networks.

They are essential for ensuring reliable wireless connectivity and good user experience.

---

# What is a Wireless Site Survey?

A Wireless Site Survey is a systematic assessment of a wireless environment.

Purpose:

* Measure Wi-Fi coverage
* Identify dead zones
* Detect interference
* Plan Access Point placement
* Improve network performance

---

# Why is a Site Survey Important?

Without a site survey:

* Coverage gaps may occur
* Performance may suffer
* Interference may increase
* Users may experience disconnections

A survey helps ensure proper wireless network design.

---

# Goals of a Site Survey

Common goals include:

* Reliable coverage
* Good signal strength
* Minimal interference
* Proper channel allocation
* Optimal Access Point placement

---

# Wireless Coverage

Coverage refers to the area where Wi-Fi signals can be received reliably.

Example:

```text id="coverage1"
Access Point
      │
Wireless Coverage Area
```

Coverage depends on:

* AP power
* Obstacles
* Building materials
* Frequency band

---

# Dead Zones

A Dead Zone is an area where Wi-Fi coverage is weak or unavailable.

Example:

```text id="dead1"
Office Floor

Strong Signal
     │
Weak Signal
     │
Dead Zone
```

Site surveys help identify these areas.

---

# Signal Strength

Signal strength indicates how strong a wireless signal is at a location.

Typically measured in:

```text id="rssi1"
dBm
```

Common values:

| Signal Strength | Quality    |
| --------------- | ---------- |
| -30 dBm         | Excellent  |
| -50 dBm         | Very Good  |
| -67 dBm         | Good       |
| -70 dBm         | Acceptable |
| -80 dBm         | Weak       |
| -90 dBm         | Poor       |

---

# RSSI

RSSI stands for:

```text id="rssi2"
Received Signal Strength Indicator
```

RSSI helps determine the strength of a received wireless signal.

Higher-quality signals generally result in better performance.

---

# Noise

Noise refers to unwanted radio signals that interfere with Wi-Fi communication.

Sources may include:

* Electronic devices
* Other wireless networks
* Industrial equipment
* Environmental interference

---

# Signal-to-Noise Ratio (SNR)

SNR stands for:

```text id="snr1"
Signal-to-Noise Ratio
```

SNR compares:

```text id="snr2"
Signal Strength
      vs
Noise Level
```

Higher SNR generally means better communication quality.

---

# Example

```text id="snr3"
Signal: -50 dBm

Noise: -90 dBm

SNR: 40 dB
```

This would generally indicate a good wireless environment.

---

# Interference

Interference occurs when unwanted signals affect wireless communication.

Common sources:

* Nearby Wi-Fi networks
* Bluetooth devices
* Microwave ovens
* Wireless cameras
* Industrial equipment

---

# Co-Channel Interference (CCI)

CCI occurs when multiple Access Points use the same channel.

Example:

```text id="cci1"
AP 1 → Channel 6

AP 2 → Channel 6
```

Too much channel sharing can reduce performance.

---

# Adjacent Channel Interference (ACI)

ACI occurs when overlapping channels interfere with each other.

Example:

```text id="aci1"
AP 1 → Channel 4

AP 2 → Channel 5
```

Proper channel planning helps avoid this issue.

---

# Channel Planning

Channel planning involves assigning channels to Access Points to reduce interference.

Benefits:

* Better performance
* Improved stability
* Reduced interference

---

# Access Point Placement

Correct AP placement is critical.

Considerations:

* Building layout
* User density
* Obstacles
* Coverage requirements
* Signal overlap

---

# Common Obstacles

Wireless signals can be affected by:

* Concrete walls
* Metal surfaces
* Elevators
* Glass
* Furniture

These obstacles may reduce signal quality.

---

# Types of Site Surveys

## Passive Survey

The survey device listens to wireless traffic.

Purpose:

* Measure coverage
* Analyze signal strength
* Identify wireless networks

---

## Active Survey

The survey device actively connects to the network.

Purpose:

* Measure performance
* Test connectivity
* Validate user experience

---

## Predictive Survey

Uses software simulations before deployment.

Purpose:

* Plan AP locations
* Estimate coverage
* Reduce deployment costs

---

# Wireless Heat Maps

Heat maps visually display wireless coverage.

Example:

```text id="heat1"
Strong Signal
      ↓
Medium Signal
      ↓
Weak Signal
```

Heat maps help administrators understand coverage distribution.

---

# Site Survey Workflow

```text id="workflow1"
Analyze Environment
        ↓
Measure Signals
        ↓
Identify Interference
        ↓
Plan Channels
        ↓
Place Access Points
        ↓
Validate Coverage
```

---

# Tools Used During Surveys

Examples include:

* Wi-Fi analyzers
* Survey software
* Spectrum analyzers
* Wireless monitoring tools

These tools help collect wireless performance data.

---

# Benefits of Site Surveys

Site surveys help:

* Improve coverage
* Increase reliability
* Reduce interference
* Optimize AP placement
* Improve user experience

---

# Real-Life Example

A company deploys new Wi-Fi infrastructure.

Before installation, engineers perform a site survey to:

* Determine AP locations
* Measure interference
* Identify dead zones
* Plan channels

The result is a more reliable wireless network.

---

# Site Surveys in Cybersecurity

Security professionals use site surveys to:

* Discover wireless devices
* Identify Rogue APs
* Detect unknown SSIDs
* Verify wireless coverage
* Improve wireless visibility

Site surveys play an important role in wireless security assessments.

---

# Summary

* Wireless Site Surveys help design and optimize Wi-Fi networks.
* They identify coverage issues, interference, and dead zones.
* RSSI measures signal strength.
* SNR measures signal quality relative to noise.
* Proper channel planning improves performance.
* Site surveys assist with AP placement and wireless troubleshooting.
* They are essential for both networking and cybersecurity professionals.
