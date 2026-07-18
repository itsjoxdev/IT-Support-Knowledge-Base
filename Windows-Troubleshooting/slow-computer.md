# Slow Computer Troubleshooting

## Overview

A slow computer is one of the most common issues reported to IT Support. This guide provides a structured approach to diagnosing and resolving performance problems on Windows systems.

---

## Symptoms

Users may report one or more of the following:

- Slow system startup
- Applications take a long time to open
- Frequent freezing or lagging
- High CPU, Memory, or Disk usage
- Slow file transfers
- Delayed response when switching between applications

---

## Possible Causes

- Too many startup applications
- Low available RAM
- High CPU usage
- Insufficient disk space
- Malware or viruses
- Outdated Windows or device drivers
- Background applications consuming resources
- Failing HDD or SSD

---

## Troubleshooting Methodology

Follow these steps in order before considering hardware replacement.

### Step 1 – Restart the Computer

A restart clears temporary processes and may resolve performance issues.

---

### Step 2 – Check Resource Usage

Open **Task Manager**:

```
Ctrl + Shift + Esc
```

Review:

- CPU Usage
- Memory Usage
- Disk Usage
- Network Usage

Identify applications consuming excessive resources.

---

### Step 3 – Disable Unnecessary Startup Programs

Open:

```
Task Manager → Startup Apps
```

Disable unnecessary applications that start automatically with Windows.

---

### Step 4 – Check Available Disk Space

Open:

```
This PC
```

Ensure the system drive (C:) has at least 15–20% free space.

---

### Step 5 – Remove Temporary Files

Open Run:

```
Windows + R
```

Type:

```
temp
```

Delete unnecessary files.

Repeat with:

```
%temp%
```

---

### Step 6 – Scan for Malware

Open:

```
Windows Security
```

Navigate to:

```
Virus & Threat Protection
```

Run a **Full Scan**.

---

### Step 7 – Install Windows Updates

Go to:

```
Settings → Windows Update
```

Install all available updates.

---

### Step 8 – Check System Health

Run Command Prompt as Administrator and execute:

```cmd
sfc /scannow
```

If Windows reports corruption, run:

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
```

---

## Useful Commands

```cmd
taskmgr
```

Opens Task Manager.

```cmd
cleanmgr
```

Launches Disk Cleanup.

```cmd
sfc /scannow
```

Scans and repairs corrupted system files.

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
```

Repairs the Windows image.

```cmd
chkdsk /f
```

Checks and repairs disk errors.

---

## Resolution

After troubleshooting:

- Remove unnecessary startup applications.
- Delete temporary files.
- Free disk space.
- Install Windows updates.
- Scan for malware.
- Repair corrupted system files.
- Upgrade RAM or replace HDD with SSD if required.

---

## Prevention

- Restart the computer regularly.
- Keep Windows updated.
- Avoid installing unnecessary software.
- Maintain at least 20% free disk space.
- Perform regular antivirus scans.
- Use SSD storage whenever possible.

---

## Related Issues

- Windows Startup Problems
- Blue Screen (BSOD)
- Windows Update Errors