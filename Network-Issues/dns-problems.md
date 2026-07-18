# DNS Troubleshooting

## Overview

The Domain Name System (DNS) translates domain names into IP addresses, allowing users to access websites and online services. DNS issues can prevent internet access even when the network connection is working properly.

---

## Symptoms

Users may experience:

- Websites do not load
- "DNS Server Not Responding" error
- Internet connection is available, but websites cannot be accessed
- Some websites work while others do not
- Ping to an IP address succeeds, but ping to a domain name fails

---

## Possible Causes

- Incorrect DNS server configuration
- Corrupted DNS cache
- Router DNS issues
- ISP DNS outage
- Firewall or antivirus interference
- Network adapter configuration problems

---

## Troubleshooting Methodology

### Step 1 – Verify Internet Connectivity

Run:

```cmd
ping 8.8.8.8
```

If the ping succeeds, the internet connection is working.

---

### Step 2 – Test DNS Resolution

Run:

```cmd
ping google.com
```

If this fails while pinging an IP works, the issue is likely DNS-related.

---

### Step 3 – Display Current DNS Configuration

Run:

```cmd
ipconfig /all
```

Verify the configured DNS servers.

---

### Step 4 – Flush the DNS Cache

Run:

```cmd
ipconfig /flushdns
```

---

### Step 5 – Renew the IP Address

Run:

```cmd
ipconfig /release
ipconfig /renew
```

---

### Step 6 – Test DNS Servers

Run:

```cmd
nslookup google.com
```

Check whether the configured DNS server returns a valid IP address.

---

### Step 7 – Change DNS Server

Use a public DNS server.

Example:

Google DNS

```
Primary: 8.8.8.8
Secondary: 8.8.4.4
```

Cloudflare DNS

```
Primary: 1.1.1.1
Secondary: 1.0.0.1
```

---

### Step 8 – Restart Networking Equipment

Restart:

- Router
- Modem
- Computer

---

## Useful Commands

```cmd
ipconfig /all
```

Display complete network configuration.

```cmd
ipconfig /flushdns
```

Clear the DNS cache.

```cmd
ipconfig /release
```

Release the current IP address.

```cmd
ipconfig /renew
```

Obtain a new IP address.

```cmd
nslookup
```

Query DNS servers.

```cmd
ping
```

Test connectivity.

```cmd
tracert
```

Trace the route to a destination.

---

## Resolution

Most DNS issues are resolved by:

- Flushing the DNS cache
- Renewing the IP address
- Changing to a reliable public DNS server
- Restarting networking equipment
- Correcting network adapter settings

---

## Prevention

- Use reliable DNS servers.
- Keep network drivers updated.
- Restart networking equipment when necessary.
- Keep Windows updated.
- Avoid unauthorized network configuration changes.

---

## Related Issues

- WiFi Problems
- Internet Not Working
- IP Configuration