# G3MIT Device Password Consolidation

This package consolidates the eight CISv4 Device Password Enabled child-policy JSON files into one Intune policy:

- G3MIT - WIN - L1 - Device Password Policy

Do not assign the original eight individual Device Password Enabled JSON policies alongside this consolidated policy. They all share the same parent setting definition and may cause Intune conflicts.

Consolidated settings:

- Device password enabled
- Alphanumeric device password required
- Minimum password complex characters
- Device password expiration: 365 days
- Device password history: 24
- Max failed attempts: 5
- Max inactivity lock: 15 minutes
- Minimum password length: 14
