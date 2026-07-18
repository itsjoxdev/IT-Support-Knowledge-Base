# Networking Commands Reference

## Overview

This document contains commonly used Windows networking commands for IT Support troubleshooting and network diagnostics.

These commands help technicians identify connectivity problems, diagnose configuration issues, and verify network communication.

---

## IP Configuration Commands

| Command | Description |
|---------|-------------|
| `ipconfig` | Display basic IP configuration |
| `ipconfig /all` | Display detailed network configuration |
| `ipconfig /release` | Release the current IP address |
| `ipconfig /renew` | Request a new IP address from DHCP |
| `ipconfig /flushdns` | Clear the DNS resolver cache |

---

## Connectivity Testing Commands

| Command | Description |
|---------|-------------|
| `ping` | Test connectivity between devices |
| `tracert` | Trace the network path to a destination |
| `pathping` | Combine ping and traceroute analysis |
| `telnet` | Test connection to a specific port |

---

## DNS Diagnostic Commands

| Command | Description |
|---------|-------------|
| `nslookup` | Query DNS records and test name resolution |
| `nslookup domain.com` | Check DNS resolution for a specific domain |

Example:

```cmd
nslookup google.com
```

---

## Network Information Commands

| Command | Description |
|---------|-------------|
| `netstat` | Display active network connections |
| `netstat -ano` | Show connections with process IDs |
| `arp -a` | Display ARP cache entries |
| `hostname` | Display the computer name |

---

## Network Reset Commands

| Command | Description |
|---------|-------------|
| `netsh winsock reset` | Reset Windows Winsock configuration |
| `netsh int ip reset` | Reset TCP/IP settings |

---

## Troubleshooting Examples

### No Internet Connection

Use:

```cmd
ipconfig
```

Check if the device has a valid IP address.

Then:

```cmd
ping 8.8.8.8
```

Test Internet connectivity.

---

### DNS Problem

Run:

```cmd
nslookup google.com
```

If DNS resolution fails:

```cmd
ipconfig /flushdns
```

---

### Network Path Issue

Run:

```cmd
tracert google.com
```

to identify where the connection fails.

---

## Common IT Support Workflow

1. Check IP configuration:

```cmd
ipconfig /all
```

2. Test local connectivity:

```cmd
ping <gateway>
```

3. Test Internet connectivity:

```cmd
ping 8.8.8.8
```

4. Test DNS:

```cmd
nslookup google.com
```

5. Analyze route:

```cmd
tracert google.com
```

---

## Related Documentation

- WiFi Problems
- DNS Problems
- IP Configuration
- Internet Connectivity Issues