# G3IT Clean Intune BitLocker JSON Import Set

This package contains cleaned Microsoft Graph beta deviceManagementConfigurationPolicy JSON payloads based on the CyberDrain CISv4 BitLocker templates provided in this chat.

Recommended import order:
1. G3IT - WIN - BL - Require Device Encryption
2. G3IT - WIN - BL - Silent Encryption Warning Behavior
3. G3IT - WIN - BL - Choose Drive Encryption Method and Cipher Strength
4. G3IT - WIN - BL - Operating System Drive Recovery
5. G3IT - WIN - BL - Fixed Drive Recovery
6. G3IT - WIN - BL - Startup Authentication

Optional/pilot policies:
7. G3IT - WIN - BL - Deny Write Access To Unencrypted Removable Drives - Optional Compliance
8. G3IT - WIN - DMA Guard - Device Enumeration Policy Block All - Optional Pilot

Do not also assign the individual CyberDrain child policies for Recovery Key, Recovery Password, TPM startup key, TPM startup PIN, TPM startup key and PIN, or Data Recovery Agent. Those overlap with the consolidated policies and can create Intune conflicts.

These files are cleaned for import/create workflows and do not include the original policy IDs, assignment links, or tenant-specific Graph URLs.
