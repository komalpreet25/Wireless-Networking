# Wi-Fi Channels and Frequencies

## Description

Wi-Fi networks operate using radio frequencies divided into channels.

These channels determine how wireless data is transmitted between devices and Access Points.

Understanding channels and frequencies is important for network performance, interference reduction, and wireless security analysis.

---

# What are Wi-Fi Frequencies?

Wi-Fi uses radio waves to transmit data.

Common frequency bands:

* 2.4 GHz
* 5 GHz
* 6 GHz (Wi-Fi 6E and Wi-Fi 7)

Each band has different characteristics like range, speed, and interference levels.

---

# 2.4 GHz Band

## Features

* Longer range
* Slower speed
* High interference

## Advantages

* Works through walls better
* Wide coverage area

## Disadvantages

* Very crowded
* Overlapping channels

---

## 2.4 GHz Channels

In most countries, 2.4 GHz has 13 channels (India included).

Each channel is 5 MHz apart.

However, channels overlap with each other.

---

## Non-Overlapping Channels

Only 3 channels do not overlap:

```text id="ch1"
Channel 1
Channel 6
Channel 11
```

These are the most recommended channels for stable Wi-Fi.

---

# 5 GHz Band

## Features

* Higher speed
* Lower interference
* Shorter range

## Advantages

* More channels available
* Better performance

## Disadvantages

* Reduced coverage through walls
* Higher power consumption

---

## 5 GHz Channels

* Many non-overlapping channels
* Supports wider channel widths (20/40/80/160 MHz)
* Used in modern routers and devices

---

# 6 GHz Band (Wi-Fi 6E and Wi-Fi 7)

## Features

* Very high speed
* Very low interference
* Large number of channels

## Advantages

* Clean spectrum
* Ideal for high-performance applications

## Disadvantages

* Short range
* Limited device support (older devices not compatible)

---

# What is a Channel?

A channel is a specific range of frequencies within a band.

Example:

```text id="channel1"
2.4 GHz Band
Channel 6 → specific frequency range
```

Devices communicate on the same channel to exchange data.

---

# Channel Overlap (2.4 GHz Problem)

In 2.4 GHz, channels overlap with each other.

Example:

```text id="overlap1"
Channel 1 overlaps with Channel 2, 3, 4, 5
```

This causes:

* Interference
* Packet loss
* Reduced speed

---

# Why Channels 1, 6, 11 are Important?

These channels do not overlap.

```text id="nonoverlap"
1 ---- 6 ---- 11
```

Using these reduces interference and improves performance.

---

# Channel Width

Channel width determines how much data can be transmitted.

Common widths:

| Width   | Description               |
| ------- | ------------------------- |
| 20 MHz  | Stable, less interference |
| 40 MHz  | Moderate speed            |
| 80 MHz  | High speed                |
| 160 MHz | Very high speed           |

---

# 2.4 GHz vs 5 GHz vs 6 GHz

| Feature      | 2.4 GHz | 5 GHz  | 6 GHz     |
| ------------ | ------- | ------ | --------- |
| Speed        | Low     | High   | Very High |
| Range        | High    | Medium | Low       |
| Interference | High    | Medium | Very Low  |
| Channels     | Few     | Many   | Very Many |

---

# Interference in Wi-Fi

Interference happens when multiple signals overlap.

Causes:

* Nearby Wi-Fi networks
* Bluetooth devices
* Microwave ovens
* Wireless cameras
* Physical obstacles

---

# How Channels Affect Performance

Wrong channel selection leads to:

* Slow internet
* Packet loss
* Connection drops

Proper channel selection improves:

* Speed
* Stability
* Range efficiency

---

# Auto Channel Selection

Modern routers can automatically select the best channel.

Advantages:

* Easy setup
* Reduces manual configuration

Disadvantages:

* May not always choose optimal channel

---

# DFS Channels

DFS (Dynamic Frequency Selection) channels exist in the 5 GHz band.

These channels:

* Share spectrum with radar systems
* Require monitoring for radar signals
* May switch automatically if radar is detected

---

# Real-Life Example

Home Wi-Fi setup:

```text id="homewifi"
Router → Channel 6 (2.4 GHz)
Phone → Connected
Laptop → Connected
TV → Connected
```

If neighbor Wi-Fi uses Channel 6 too:

* Interference increases
* Performance drops

Solution:

* Switch to Channel 1 or 11

---

# Wi-Fi Channel Usage in Cities

In crowded areas:

* Many overlapping 2.4 GHz networks
* 5 GHz becomes more useful
* 6 GHz is best for performance

---

# Channel Selection Best Practices

* Use 2.4 GHz channels 1, 6, 11
* Prefer 5 GHz for speed
* Use 6 GHz for modern devices
* Avoid crowded channels
* Use Wi-Fi analyzer tools

---

# Wi-Fi Analyzer Tools

Common tools:

* Wireshark
* NetSpot
* WiFi Analyzer (Android)
* Acrylic Wi-Fi

These tools help visualize:

* Channels
* Signal strength
* Interference

---

# Channels in Cybersecurity

Security professionals use channel analysis to:

* Detect rogue networks
* Identify interference sources
* Analyze wireless environments
* Optimize penetration testing setup
* Monitor suspicious Wi-Fi activity

---

# Summary

* Wi-Fi uses frequency bands divided into channels.
* 2.4 GHz has longer range but more interference.
* 5 GHz provides better speed and less interference.
* 6 GHz is the fastest and cleanest band.
* Channels 1, 6, and 11 are non-overlapping in 2.4 GHz.
* Channel selection directly affects Wi-Fi performance.
* Understanding channels is essential for wireless networking and security.
