# IP Configuration Troubleshooting

## Overview

IP configuration issues prevent a computer from communicating with devices on the local network or accessing the Internet. This guide explains how to diagnose and resolve common IP-related problems on Windows systems.

---

## Symptoms

Users may experience:

- No Internet access
- "Unidentified Network"
- "No valid IP configuration"
- Limited connectivity
- Unable to reach network resources
- Automatic Private IP Address (169.254.x.x)

---

## Possible Causes

- DHCP server unavailable
- Incorrect static IP configuration
- IP address conflict
- Faulty router or switch
- Network adapter issues
- Corrupted TCP/IP settings

---

## Troubleshooting Methodology

### Step 1 – Check Current IP Configuration

Open Command Prompt:

```cmd
ipconfig
```

Verify:

- IPv4 Address
- Default Gateway
- Subnet Mask

---

### Step 2 – Display Detailed Configuration

Run:

```cmd
ipconfig /all
```

Check:

- DHCP Enabled
- DNS Servers
- MAC Address
- Lease Information

---

## Network Configuration Overview

Use Windows Network Settings to verify adapter status, connection details, and network configuration.

![Network Settings](../Screenshots/network-settings.png)

---

### Step 3 – Identify APIPA Address

If the computer receives an address like:

```
169.254.x.x
```

This usually indicates that Windows could not obtain an IP address from the DHCP server.

---

### Step 4 – Renew the IP Address

Run:

```cmd
ipconfig /release
ipconfig /renew
```

---

### Step 5 – Check Network Adapter

Open:

```
Device Manager
```

Verify that the network adapter:

- Is enabled
- Has no warning icons
- Uses the latest driver

---

### Step 6 – Verify TCP/IP Settings

Open:

```
Network Connections
```

Select the adapter.

Open:

```
Internet Protocol Version 4 (TCP/IPv4)
```

Confirm:

- Obtain an IP address automatically

or

- Verify the configured static IP settings

---

### Step 7 – Test Gateway Connectivity

Run:

```cmd
ping <Default Gateway IP>
```

Example:

```cmd
ping 192.168.1.1
```

---

### Step 8 – Reset TCP/IP

Run Command Prompt as Administrator:

```cmd
netsh int ip reset

netsh winsock reset
```

Restart the computer.

---

## Useful Commands

```cmd
ipconfig
```

Display current IP configuration.

```cmd
ipconfig /all
```

Display complete network configuration.

```cmd
ipconfig /release
```

Release the current IP address.

```cmd
ipconfig /renew
```

Request a new IP address.

```cmd
arp -a
```

Display the ARP cache.

```cmd
netsh int ip reset
```

Reset TCP/IP settings.

```cmd
netsh winsock reset
```

Reset the Windows networking stack.

```cmd
ping
```

Test connectivity.

---

## Resolution

Common solutions include:

- Renewing the IP address
- Restarting the router
- Correcting static IP settings
- Enabling DHCP
- Resetting TCP/IP
- Updating network drivers

---

## Prevention

- Use DHCP unless static addressing is required.
- Avoid duplicate IP addresses.
- Keep network drivers updated.
- Restart networking equipment when necessary.
- Document static IP assignments.

---

## Related Issues

- WiFi Problems
- DNS Problems
- Internet Not Working