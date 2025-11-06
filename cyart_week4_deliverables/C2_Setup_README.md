# C2_Setup_README

**Lab prerequisites**
- Isolated lab network
- Cobalt Strike teamserver (lab license or alternative open-source C2)
- Valid TLS cert for listener (lab-generated)
- Windows VM for target and Kali attacker VM

**Steps**
1. Configure Cobalt Strike teamserver on attacker host.
2. Create HTTPS listener with staging disabled (stageless).
3. Generate PowerShell stageless beacon one-liner via PoshC2 or Cobalt Strike.
4. Deliver beacon via simulated phishing payload (Evilginx2 landing page or email simulation).
5. On connection, verify session and interact with the beacon via the teamserver console.

**Safety**
- Do not use any of these steps against third-party or production systems.
