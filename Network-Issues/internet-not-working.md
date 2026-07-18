# Internet Not Working Troubleshooting

## Overview

Internet connectivity issues are among the most common incidents handled by IT Support teams. This guide provides a step-by-step process to diagnose and resolve internet connection problems on Windows systems.

---

## Symptoms

Users may experience:

- No Internet access
- Websites fail to load
- Applications cannot connect online
- Limited or no connectivity
- Yellow warning icon on the network connection
- Network connected but no Internet

---

## Possible Causes

- ISP outage
- Router or modem failure
- Incorrect IP configuration
- DNS problems
- Faulty network cable
- Disabled network adapter
- Firewall or antivirus blocking connections
- Driver issues

---

## Troubleshooting Methodology

### Step 1 – Check Physical Connections

Verify:

- Ethernet cable is connected securely
- Router and modem are powered on
- Network LEDs are active

---

### Step 2 – Verify Network Adapter

Open:

```
Settings → Network & Internet
```

Ensure the network adapter is enabled.

---

### Step 3 – Restart Network Equipment

Restart:

- Computer
- Router
- Modem

Wait 2–3 minutes before testing again.

---

### Step 4 – Check IP Configuration

Run:

```cmd
ipconfig
```

Confirm the computer has a valid IPv4 address.

---

### Step 5 – Test Local Network

Ping the default gateway:

```cmd
ping 192.168.1.1
```

Replace the IP address with your router's gateway if different.

---

### Step 6 – Test Internet Connectivity

Run:

```cmd
ping 8.8.8.8
```

If successful, Internet connectivity exists.

---

### Step 7 – Test DNS Resolution

Run:

```cmd
ping google.com
```

If this fails while pinging 8.8.8.8 succeeds, the issue is DNS-related.

---

### Step 8 – Renew Network Configuration

Run:

```cmd
ipconfig /release

ipconfig /renew

ipconfig /flushdns
```

---

### Step 9 – Reset Network Stack

Run Command Prompt as Administrator:

```cmd
netsh winsock reset

netsh int ip reset
```

Restart the computer.

---

### Step 10 – Check for ISP Issues

If all local troubleshooting steps fail:

- Test another device on the same network.
- Contact the Internet Service Provider (ISP).

---

## Useful Commands

```cmd
ipconfig
```

Display IP configuration.

```cmd
ipconfig /all
```

Display detailed network information.

```cmd
ipconfig /release
```

Release the current IP address.

```cmd
ipconfig /renew
```

Renew the current IP address.

```cmd
ipconfig /flushdns
```

Clear the DNS cache.

```cmd
ping
```

Test network connectivity.

```cmd
tracert
```

Trace the network path.

```cmd
netsh winsock reset
```

Reset Winsock.

```cmd
netsh int ip reset
```

Reset TCP/IP settings.

---

## Resolution

Most Internet connectivity issues are resolved by:

- Restarting networking equipment
- Renewing the IP address
- Flushing the DNS cache
- Resetting the network stack
- Updating network drivers
- Resolving ISP outages

---

## Prevention

- Keep Windows updated.
- Update network drivers regularly.
- Restart networking equipment periodically.
- Avoid unauthorized network configuration changes.
- Use reliable networking hardware.

---

## Related Issues

- WiFi Problems
- DNS Problems
- IP Configuration