# Email Troubleshooting

## Overview

Email issues are among the most frequent requests handled by IT Support teams. This guide provides a structured approach to diagnosing and resolving common email problems.

---

## Symptoms

Users may experience:

- Unable to send emails
- Unable to receive emails
- Login failures
- Outlook not responding
- Email synchronization issues
- Attachments fail to send
- Mailbox is full

---

## Possible Causes

- Incorrect username or password
- Internet connectivity issues
- Incorrect email server settings
- Full mailbox
- Outlook profile corruption
- Firewall or antivirus interference
- Email service outage

---

## Troubleshooting Methodology

### Step 1 – Verify Internet Connection

Ensure the computer has Internet access.

Run:

```cmd
ping google.com
```

If the test fails, troubleshoot the network connection first.

---

### Step 2 – Verify User Credentials

Confirm:

- Correct email address
- Correct password
- Multi-Factor Authentication (MFA), if enabled

---

### Step 3 – Check Mailbox Storage

Verify that the mailbox has available storage.

Delete unnecessary emails if the mailbox is full.

---

### Step 4 – Restart the Email Application

Close and reopen the email client.

If using Outlook, restart the computer if necessary.

---

### Step 5 – Verify Email Server Settings

Check:

- Incoming server (IMAP/POP3)
- Outgoing server (SMTP)
- Port numbers
- Encryption settings

---

### Step 6 – Test Webmail Access

Sign in through the organization's webmail portal.

If webmail works but Outlook does not, the issue is likely with the email client.

---

### Step 7 – Repair the Email Profile

If Outlook continues to fail:

- Create a new Outlook profile.
- Reconfigure the email account.

---

### Step 8 – Check Service Status

Verify whether the email service is experiencing an outage.

If using Microsoft 365 or Google Workspace, check the service health dashboard.

---

## Useful Commands

```cmd
ping
```

Test Internet connectivity.

```cmd
ipconfig /flushdns
```

Clear the DNS cache.

```cmd
outlook.exe /safe
```

Start Microsoft Outlook in Safe Mode.

---

## Resolution

Most email issues can be resolved by:

- Correcting login credentials
- Restoring Internet connectivity
- Updating server settings
- Restarting or repairing Outlook
- Freeing mailbox storage

---

## Prevention

- Keep Outlook and Windows updated.
- Use strong passwords and enable MFA.
- Monitor mailbox storage.
- Avoid opening suspicious email attachments.
- Regularly archive old emails.

---

## Escalation

Escalate the issue if:

- The email server is unavailable.
- Multiple users are affected.
- Mailboxes cannot be accessed after troubleshooting.
- A security incident (phishing or account compromise) is suspected.

---

## Related Issues

- Password Reset
- Account Lockout
- DNS Problems