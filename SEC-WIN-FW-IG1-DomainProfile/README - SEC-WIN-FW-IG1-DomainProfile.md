# SEC-WIN-FW-IG1-DomainProfile

This JSON consolidates the CISv4 WIN L1 Domain Network Firewall child policies into one G3MIT-standard Intune policy.

## Consolidated Policy Name
SEC-WIN-FW-IG1-DomainProfile

## Assignment
Include: SEC-WIN-CISIG1-STD-Dynamic  
Exclude: SEC-WIN-CISIG1-EXC-Assigned

## Consolidated Settings
- Domain firewall enabled: True
- Default inbound action: Block
- Default outbound action: Allow
- Disable inbound notifications: True
- Enable log dropped packets: True
- Enable log successful connections: True
- Log maximum file size: 16384 KB
- Log path: %systemroot%\system32\LogFiles\Firewall\pfirewall.log

## Do Not Also Assign
Do not assign the six original Domain Network Firewall child policies alongside this consolidated policy because they share the same parent setting definition and can create Intune conflicts.
