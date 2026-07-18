# WiFi Connectivity Troubleshooting

## Overview

WiFi connectivity issues are among the most common problems reported to IT Support. This guide provides a structured approach to diagnosing and resolving wireless network problems on Windows systems.

---

## Symptoms

Users may experience:

- Unable to connect to WiFi
- No Internet access
- Slow Internet speed
- Frequent disconnections
- Limited connectivity
- WiFi network not visible

---

## Possible Causes

- WiFi adapter disabled
- Incorrect WiFi password
- Weak wireless signal
- Router or modem issues
- Outdated network drivers
- Incorrect IP or DNS configuration
- ISP outage

---

## Troubleshooting Methodology

### Step 1 – Check WiFi Status

Verify that WiFi is enabled.

Go to:

```
Settings → Network & Internet → WiFi
```

Ensure WiFi is turned on.

---

### Step 2 – Verify Airplane Mode

Check that Airplane Mode is disabled.

---

### Step 3 – Restart Devices

Restart:

- Computer
- Router
- Modem

Wait 2–3 minutes before reconnecting.

---

### Step 4 – Forget and Reconnect

Open:

```
Settings → WiFi → Manage Known Networks
```

Forget the network and reconnect using the correct password.

---

### Step 5 – Check IP Configuration

Open Command Prompt:

```cmd
ipconfig
```

Verify the computer has a valid IPv4 address.

---

### Step 6 – Renew IP Address

Run:

```cmd
ipconfig /release
ipconfig /renew
```

---

### Step 7 – Test Network Connectivity

Ping the local router:

```cmd
ping 192.168.1.1
```

Then test Internet connectivity:

```cmd
ping 8.8.8.8
```

Finally test DNS resolution:

```cmd
ping google.com
```

---

### Step 8 – Reset Network Stack

Run Command Prompt as Administrator:

```cmd
netsh winsock reset

netsh int ip reset

ipconfig /flushdns
```

Restart the computer.

---

### Step 9 – Update Network Driver

Open:

```
Device Manager
```

Update the Wireless Network Adapter driver.

---

## Useful Commands

```cmd
ipconfig
```

Display network configuration.

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

Request a new IP address.

```cmd
ipconfig /flushdns
```

Clear the DNS cache.

```cmd
ping
```

Test connectivity.

```cmd
tracert
```

Trace the network route.

```cmd
netsh winsock reset
```

Reset the Windows network stack.

---

## Resolution

Most WiFi issues are resolved by:

- Restarting networking equipment
- Renewing the IP address
- Resetting the network stack
- Updating drivers
- Correcting WiFi credentials
- Resolving router configuration issues

---

## Prevention

- Keep network drivers updated.
- Restart networking equipment regularly.
- Secure WiFi with a strong password.
- Avoid signal interference.
- Keep Windows updated.

---

## Related Issues

- DNS Problems
- IP Configuration
- Internet Not Working