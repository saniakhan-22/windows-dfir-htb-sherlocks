#  HTB Sherlock: Campfire-2
 * **Platform:** Hack The Box

* **Category:** DFIR

* **Difficulty:** Easy

* **Focus:** Windows Event Log Analysis

* **Tools:** Windows Event Viewer

## Scenario
Investigate a suspicious Kerberos ticket request involving an unused administrator account and determine whether it indicates AS-REP Roasting.

## Investigation
- **Artifact:** 'Security.evtx' - Domain Controller Security Log.
- ""Objective:** Identify suspicoius Kerberos authentication activity and correlate related events.
- **Key Event ID:** '4768' - Kerberos Ticket Granting (TGT) request.
- **Detection indicator:** 'PreAuthType = 0 , which can indicate a request for an account without Kerberos pre-authentication.

## Findings
- **Timestamp (UTC):** '2024-05-29 06:36:40'
- **Target Account:** 'arthur.kyle'
- **Source IP:** '172.17.79.129'
- **Investigation Focus:** Suspicious Kerberos ticket request associated with potential AS-REP Roasting.

## Skills Learnt
- Active Directory attack analysis
- AS-REP Roasting detection and analysis
- Windows Event Log analysis
- Timeline creation and event correlation
- Correlation of multiple artifacts to reconstruct activity

## Key Takeaway
Learned how Domain Controller Security logs can help potential AS-REP Roasting and how event correlation supports incident investigatiom.

## MITRE ATT&CK
- **T1558.004** - Steal or Forge Kerberos Tickets: AS-REP Roasting

## Evidence
![Suspicous Event](campfire-2-suspicious-event.png)
