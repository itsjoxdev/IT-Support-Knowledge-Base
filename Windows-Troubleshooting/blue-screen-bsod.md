# Blue Screen of Death (BSOD) Troubleshooting

## Overview

The Blue Screen of Death (BSOD) is a critical Windows error that causes the operating system to stop unexpectedly to prevent further damage. This guide explains common causes, troubleshooting steps, and possible solutions.

---

## Symptoms

Users may experience:

- Blue screen with an error message
- Automatic system restart
- Frequent crashes
- Windows fails to boot
- Error codes such as:
  - CRITICAL_PROCESS_DIED
  - MEMORY_MANAGEMENT
  - IRQL_NOT_LESS_OR_EQUAL
  - SYSTEM_SERVICE_EXCEPTION

---

## Possible Causes

- Corrupted system files
- Faulty RAM
- Outdated or incompatible drivers
- Windows update issues
- Hard disk errors
- Overheating
- Hardware failure

---

## Troubleshooting Methodology

### Step 1 – Record the Error Code

Write down the stop code displayed on the blue screen.

Example:

```
MEMORY_MANAGEMENT
```

---

### Step 2 – Restart the Computer

Check whether the issue occurs again.

---

### Step 3 – Boot into Safe Mode

If Windows cannot boot normally:

```
Settings → Recovery → Advanced Startup
```

Choose:

```
Safe Mode
```

---

### Step 4 – Check Windows Updates

Go to:

```
Settings → Windows Update
```

Install all available updates.

---

### Step 5 – Update Device Drivers

Open:

```
Device Manager
```

Update drivers for:

- Display Adapter
- Storage Controller
- Network Adapter

---

### Step 6 – Check System Files

Run Command Prompt as Administrator:

```cmd
sfc /scannow
```

Then:

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
```

---

### Step 7 – Check Disk Errors

Run:

```cmd
chkdsk C: /f
```

Restart the computer if prompted.

---

### Step 8 – Test Memory

Press:

```
Windows + R
```

Type:

```
mdsched.exe
```

Restart and allow Windows Memory Diagnostic to check RAM.

---

## Useful Commands

```cmd
sfc /scannow
```

Repair system files.

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
```

Repair Windows image.

```cmd
chkdsk /f
```

Check and repair disk errors.

```cmd
mdsched.exe
```

Run Windows Memory Diagnostic.

---

## Resolution

Depending on the root cause:

- Update drivers
- Repair Windows files
- Replace faulty RAM
- Repair disk errors
- Remove problematic software
- Install pending Windows updates

---

## Prevention

- Keep Windows updated.
- Install drivers from trusted sources.
- Scan regularly for malware.
- Monitor hardware temperatures.
- Shut down the computer properly.
- Back up important files regularly.

---

## Related Issues

- Slow Computer
- Startup Problems
- Windows Update Errors