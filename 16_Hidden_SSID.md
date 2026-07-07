# Hidden SSID

## Description

A Hidden SSID is a wireless network whose **network name (SSID)** is not broadcast in Beacon Frames.

Although the network still exists and functions normally, its name is not automatically displayed in the list of available Wi-Fi networks on nearby devices.

A Hidden SSID provides **less visibility**, but it **should not be considered a strong security feature**.

---

# What is an SSID?

SSID stands for:

```text id="ssid1"
Service Set Identifier
```

It is the name of a Wi-Fi network.

Examples:

* Home_WiFi
* Office_Network
* Coffee_Shop

---

# What is a Hidden SSID?

A Hidden SSID is a Wi-Fi network configured **not to advertise its network name** in Beacon Frames.

Example:

Normal Wi-Fi:

```text id="normal1"
SSID:
Office_WiFi
```

Hidden Wi-Fi:

```text id="hidden1"
SSID:
<Hidden>
```

The Access Point still sends Beacon Frames, but the SSID field is left blank or omitted.

---

# Normal SSID Broadcast

In a normal wireless network:

```text id="broadcast1"
Access Point
      │
Beacon Frame
      │
SSID = Office_WiFi
```

Nearby devices automatically display the network name.

---

# Hidden SSID Broadcast

With a Hidden SSID:

```text id="broadcast2"
Access Point
      │
Beacon Frame
      │
SSID = Hidden
```

The network remains active, but the name is not shown in the available Wi-Fi list.

---

# How Do Users Connect?

To join a Hidden SSID network, users usually need to enter:

* Network Name (SSID)
* Security Type
* Wi-Fi Password

Because the SSID is not broadcast, devices cannot automatically discover the network name.

---

# Probe Requests

When a device wants to reconnect to a Hidden SSID, it may send a **Probe Request** asking specifically for that network.

Example:

```text id="probe1"
Laptop
   │
Probe Request:
"Office_WiFi"
   │
Access Point
```

If the Access Point recognizes the requested SSID, it responds accordingly.

---

# Advantages of Hidden SSID

Some administrators choose Hidden SSIDs to:

* Reduce casual visibility
* Keep the network name out of automatic Wi-Fi lists
* Minimize accidental connection attempts

However, these are convenience benefits rather than strong security protections.

---

# Limitations

Hidden SSIDs have several limitations:

* The network is still active.
* Beacon Frames are still transmitted.
* Authorized clients may reveal the SSID when reconnecting.
* Users must manually configure devices.

Therefore, hiding an SSID does not prevent a determined observer from identifying the network.

---

# Hidden SSID vs Visible SSID

| Feature                     | Visible SSID | Hidden SSID |
| --------------------------- | ------------ | ----------- |
| Appears in Wi-Fi List       | Yes          | No          |
| Manual Configuration Needed | No           | Yes         |
| Network Exists              | Yes          | Yes         |
| Strong Security Feature     | No           | No          |

---

# Hidden SSID in Wireshark

During wireless analysis, Wireshark may show:

* Beacon Frames
* Probe Requests
* Probe Responses

These frames can help explain how devices discover and reconnect to Hidden SSID networks.

---

# Common Misconceptions

### Myth

A Hidden SSID makes a Wi-Fi network secure.

**Reality**

No.

Hiding the network name alone does not provide strong security.

---

### Myth

A Hidden SSID cannot be found.

**Reality**

The network still communicates using IEEE 802.11 management frames, and its existence can still be observed during wireless analysis.

---

### Myth

A Hidden SSID replaces WPA2 or WPA3.

**Reality**

No.

Strong authentication and encryption (such as WPA2 or WPA3) are still required.

---

# Best Security Practices

For better wireless security:

* Use WPA3 whenever possible.
* If WPA3 is unavailable, use WPA2 with AES.
* Choose a strong, unique Wi-Fi password.
* Keep router firmware updated.
* Disable outdated protocols such as WEP.

A Hidden SSID may reduce visibility, but it should not be relied upon as the primary security measure.

---

# Real-Life Example

A company chooses to hide its guest Wi-Fi SSID.

Employees already know the network name and configure it manually.

Visitors who scan for nearby Wi-Fi networks do not automatically see the guest network listed.

---

# Hidden SSID in Cybersecurity

Security professionals study Hidden SSIDs to:

* Understand Wi-Fi discovery
* Analyze Beacon and Probe frames
* Troubleshoot wireless connectivity
* Learn IEEE 802.11 management behavior

Understanding Hidden SSIDs helps explain how wireless clients locate and join networks.

---

# Summary

* A Hidden SSID does not broadcast its network name in Beacon Frames.
* The network still exists and continues wireless communication.
* Users generally connect by manually entering the SSID and password.
* Hidden SSIDs reduce visibility but do not provide strong security.
* WPA2 or WPA3 with a strong password should always be used for effective wireless protection.
* Understanding Hidden SSIDs is useful for networking, Wireshark analysis, and cybersecurity.
