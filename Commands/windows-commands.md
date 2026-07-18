# Windows Commands Reference

## Overview

This document contains commonly used Windows commands for IT Support troubleshooting, system diagnostics, and maintenance tasks.

These commands help technicians analyze operating system issues, manage services, repair system files, and collect system information.

---

# System Information Commands

| Command | Description |
|---------|-------------|
| `systeminfo` | Display detailed Windows system information |
| `hostname` | Display the computer name |
| `whoami` | Display the current logged-in user |
| `ver` | Display Windows version |

---

# Process & Performance Commands

| Command | Description |
|---------|-------------|
| `taskmgr` | Open Task Manager |
| `tasklist` | Display running processes |
| `taskkill` | Terminate a running process |
| `perfmon` | Open Performance Monitor |

Examples:

```cmd
tasklist
```

```cmd
taskkill /PID 1234 /F
```

---

# Windows Repair Commands

| Command | Description |
|---------|-------------|
| `sfc /scannow` | Scan and repair corrupted system files |
| `DISM /Online /Cleanup-Image /RestoreHealth` | Repair Windows image corruption |
| `chkdsk /f` | Check and repair disk errors |

Examples:

```cmd
sfc /scannow
```

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
```

```cmd
chkdsk C: /f
```

---

# Startup & Boot Troubleshooting Commands

| Command | Description |
|---------|-------------|
| `bootrec /fixmbr` | Repair Master Boot Record |
| `bootrec /fixboot` | Repair boot sector |
| `bootrec /scanos` | Scan for Windows installations |
| `bootrec /rebuildbcd` | Rebuild Boot Configuration Data |

---

# Device Management Commands

| Command | Description |
|---------|-------------|
| `devmgmt.msc` | Open Device Manager |
| `msinfo32` | Open System Information |
| `dxdiag` | Open DirectX Diagnostic Tool |

---

# Windows Services Commands

| Command | Description |
|---------|-------------|
| `services.msc` | Open Windows Services Manager |
| `eventvwr.msc` | Open Event Viewer |
| `msconfig` | Open System Configuration |

---

# User Account Commands

| Command | Description |
|---------|-------------|
| `net user` | Display local user accounts |
| `net user username password` | Change user password |
| `control userpasswords2` | Open advanced user account settings |

Example:

```cmd
net user admin NewPassword123
```

---

# Disk Management Commands

| Command | Description |
|---------|-------------|
| `diskmgmt.msc` | Open Disk Management |
| `cleanmgr` | Open Disk Cleanup |
| `defrag` | Analyze or optimize drives |

---

# Network Related Commands

| Command | Description |
|---------|-------------|
| `ipconfig` | Display IP configuration |
| `ping` | Test network connectivity |
| `tracert` | Trace network route |
| `nslookup` | Test DNS resolution |
| `netstat` | Display active connections |

---

# Security Commands

| Command | Description |
|---------|-------------|
| `Windows Security` | Open Microsoft Defender |
| `mrt` | Run Microsoft Malicious Software Removal Tool |
| `gpupdate /force` | Refresh Group Policy settings |

---

# Useful IT Support Shortcuts

| Command | Description |
|---------|-------------|
| `cmd` | Open Command Prompt |
| `powershell` | Open PowerShell |
| `control` | Open Control Panel |
| `appwiz.cpl` | Open Programs and Features |
| `ncpa.cpl` | Open Network Connections |
| `inetcpl.cpl` | Open Internet Options |

---

# Common Troubleshooting Workflow

## Slow Computer

```cmd
taskmgr
```

Check CPU, Memory, and Disk usage.

---

## Corrupted Windows Files

Run:

```cmd
sfc /scannow
```

Then:

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
```

---

## Hardware Detection Problems

Open:

```cmd
devmgmt.msc
```

Check drivers and hardware status.

---

## System Errors Investigation

Open:

```cmd
eventvwr.msc
```

Review Windows logs.

---

## Best Practices

- Run administrative commands using Command Prompt as Administrator.
- Document commands used during troubleshooting.
- Verify the impact of commands before execution.
- Avoid changing system settings without authorization.

---

## Related Documentation

- Slow Computer
- Blue Screen (BSOD)
- Startup Problems
- Windows Update Errors
- Hardware Troubleshooting Checklist