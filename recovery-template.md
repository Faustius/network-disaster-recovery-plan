# 🚨 Network Disaster Recovery Protocol (The "Red Binder")

> **Organization:** [INSERT COMPANY NAME]
> **Last Updated:** [DATE]
> **Status:** LIVE

## 🛑 Trigger Events (When to use this)
Do not use this for a slow printer. Use this for:
1.  **Total ISP Failure:** Primary internet is down hard.
2.  **Ransomware:** Files are encrypted or "funny" extensions appear.
3.  **Server Crash:** Primary Domain Controller or File Server is unresponsive.
4.  **Physical Disaster:** Fire, flood, or prolonged power loss.

---

## 📞 Chain of Command (Who to call)
*If the house is on fire, don't email. Call.*

| Role | Name | Phone | Responsibility |
| :--- | :--- | :--- | :--- |
| **Incident Commander** | [Name] | [Phone] | Makes the final call on "Shut Down" vs "Wait". |
| **Technical Lead** | [Monadic / IT Lead] | [Phone] | Executes the technical fix. |
| **Comms Officer** | [Name] | [Phone] | Talks to employees/clients (Control the narrative). |

---

## 🛠 Protocol A: The "Cyber Event" (Ransomware/Breach)
*Symptoms: Ransom note, locked files, mouse moving on its own.*

1.  **SEVER THE CORD:**
    - [ ] Physically unplug the Ethernet cable from the Firewall/Router (WAN Port).
    - [ ] Turn off Wi-Fi access points if possible.
    - [ ] **DO NOT** turn off the infected server (We need the RAM data for forensics). Just disconnect it from the network.
2.  **ISOLATE:**
    - [ ] Instruct all employees to turn off their workstations immediately.
3.  **CONTACT:**
    - [ ] Call Monadic Engineering / Cyber Insurance Provider.
4.  **WAIT:**
    - [ ] Do not attempt to reboot or run antivirus until instructed.

---

## 🛠 Protocol B: The "ISP Blackout" (Internet Down)
*Symptoms: "No Internet" dino game.*

1.  **VERIFY:**
    - [ ] Check `downdetector.com` on a cell phone.
    - [ ] Reboot the Modem/ONT (Wait 2 minutes).
2.  **FAILOVER (If equipped):**
    - [ ] Verify LTE/5G Backup has engaged on the Firewall.
3.  **HOTSPOT PROTOCOL:**
    - [ ] Critical staff (Payroll/Dispatch) switch to mobile hotspots.
    - [ ] Non-critical staff switch to offline tasks (Filing/Inventory).

---

## 🛠 Protocol C: The "Iron Restore" (Server Death)
*Symptoms: Blue Screen of Death, Hardware smoke, Water damage.*

1.  **ASSESS:**
    - [ ] Is it the Hard Drives or the Motherboard?
2.  **VIRTUALIZE (The Monadic BDR):**
    - [ ] Spin up the local backup image as a virtual machine.
    - [ ] *Target Time to Recovery:* 1 Hour.
3.  **CLOUD FAILOVER (Total Loss):**
    - [ ] If the building is gone, initialize Cloud Recovery.
    - [ ] *Target Time to Recovery:* 4 Hours.

---

## 📝 Asset Inventory (Know what you have)
| Device Name | IP Address | Function | Login Location |
| :--- | :--- | :--- | :--- |
| **Firewall** | 192.168.1.1 | Security Gateway | [Password Manager Link] |
| **Server-01** | 192.168.1.10 | Domain Controller | [Password Manager Link] |
| **Switch-01** | 192.168.1.2 | Core Switch | [Password Manager Link] |

---
*Template provided by [Monadic Engineering](https://www.monadic-llc.com).*
