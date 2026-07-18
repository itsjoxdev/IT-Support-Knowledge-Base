# Account Lockout Troubleshooting

## Overview

Account lockout occurs when a user exceeds the maximum number of failed login attempts defined by the organization's security policy. This guide explains how to identify, troubleshoot, and resolve account lockout issues.

---

## Symptoms

Users may experience:

- "Your account has been locked."
- Unable to sign in despite using the correct password.
- Login attempts are rejected immediately.
- Repeated prompts for credentials.

---

## Possible Causes

- Multiple incorrect password attempts
- Cached old credentials
- Expired password
- Incorrect password saved on another device
- Mapped network drives using old credentials
- Mobile devices repeatedly trying to authenticate
- Security policy enforcement

---

## Troubleshooting Methodology

### Step 1 – Verify User Identity

Confirm the user's identity according to company policy before making any account changes.

---

### Step 2 – Confirm the Lockout

Verify:

- Username is correct.
- The account is actually locked.
- The user is attempting to access the correct system.

---

### Step 3 – Check for Saved Credentials

Ask the user to check for:

- Saved browser passwords
- Windows Credential Manager entries
- Email applications
- Mobile devices
- VPN clients

Old saved passwords may repeatedly trigger account lockout.

---

### Step 4 – Unlock the Account

Unlock the account using the organization's approved identity management system.

If required, reset the user's password.

---

### Step 5 – Test Login

Ask the user to:

- Sign in again.
- Verify access to all required systems.
- Update saved passwords on all devices.

---

## Best Practices

- Verify user identity before unlocking any account.
- Encourage users to use a password manager.
- Enable Multi-Factor Authentication (MFA).
- Remove outdated saved credentials.

---

## Resolution

The issue is resolved when:

- The account is unlocked.
- The user successfully signs in.
- No further lockout events occur.

---

## Prevention

- Avoid repeated incorrect login attempts.
- Update passwords on all connected devices.
- Remove outdated stored credentials.
- Follow the organization's password policy.

---

## Escalation

Escalate the issue if:

- The account locks repeatedly.
- Suspicious login attempts are detected.
- Multiple user accounts are affected.
- A security incident is suspected.

---

## Related Issues

- Password Reset
- Email Issues
- Password Policy