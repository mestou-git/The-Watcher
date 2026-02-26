[[2026-02-27]]

- **Host VM:** Keep your Fedora host as the management station.
- **SIEM VM:** Deploy the **Wazuh All-in-One** VM (they provide an OVA). Allocate 4GB RAM, 2 vCPUs.
- **Target VM:** Deploy a fresh **Ubuntu Server** or **Windows 11** VM. This is your "victim" or "target" machine.
- **The Task:** Install the Wazuh agent on the Target VM. Configure it to forward logs to the SIEM VM.
- **The Test:** On the Target VM, try to `ssh` into it with the wrong password 5 times.
- **The Reward:** Go to the Wazuh dashboard on your host. Watch the alert appear in real-time.

