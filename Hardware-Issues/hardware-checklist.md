# Hardware Troubleshooting Checklist

## Overview

This checklist provides a systematic approach for diagnosing common hardware-related issues before escalating them to higher-level support or replacing components.

---

## Initial Inspection

Before troubleshooting:

- Confirm the reported issue.
- Ask when the problem started.
- Identify any recent hardware or software changes.
- Check for visible damage.
- Verify all cables are connected properly.

---

## Power Check

Verify:

- Computer is powered on.
- Power cable is connected.
- Power supply switch is on.
- Power indicator LEDs are working.

If using a laptop:

- Check battery level.
- Connect the AC adapter.
- Verify the charging indicator.

---

## Display Check

If the monitor shows no image:

- Verify monitor power.
- Check HDMI, DisplayPort, or VGA cable.
- Select the correct input source.
- Test with another monitor if available.

---

## Keyboard & Mouse

Verify:

- Device is connected correctly.
- USB port is functioning.
- Batteries are charged (wireless devices).
- Bluetooth connection is active.

---

## Storage Check

Verify:

- Disk is detected in BIOS.
- Sufficient free storage is available.
- No unusual clicking noises from HDD.
- SSD health is normal.

Useful command:

```cmd
chkdsk /f
```

---

## Memory (RAM)

Check for:

- Frequent crashes
- Random restarts
- Blue Screen errors

Run:

```cmd
mdsched.exe
```

to perform a Windows Memory Diagnostic.

---

## Network Hardware

Verify:

- Ethernet cable is connected.
- Router and modem LEDs are normal.
- Network adapter is enabled.
- WiFi adapter is working.

---

## Printer

Verify:

- Printer is powered on.
- Paper is loaded.
- Ink or toner is sufficient.
- No paper jams.
- Printer is online.

---

## Device Manager Check

Open:

```cmd
devmgmt.msc
```

Look for:

- Unknown devices
- Warning icons
- Disabled hardware

Update or reinstall drivers if necessary.

---

## Device Manager Overview

Device Manager allows IT Support technicians to view installed hardware, identify driver issues, and manage connected devices.

![Device Manager](../Screenshots/device-manager.png)

---

## Windows Updates

Verify Windows is up to date.

Go to:

```
Settings → Windows Update
```

Install all available updates.

---

## Final Verification

Before closing the ticket:

- Confirm the issue has been resolved.
- Test the affected hardware.
- Ask the user to verify normal operation.
- Document all troubleshooting steps performed.

---

## Escalation

Escalate the issue if:

- Hardware replacement is required.
- Physical damage is detected.
- The issue persists after completing all troubleshooting steps.
- Specialized repair is needed.

---

## Related Issues

- Printer Issues
- Keyboard & Mouse Issues
- Blue Screen (BSOD)