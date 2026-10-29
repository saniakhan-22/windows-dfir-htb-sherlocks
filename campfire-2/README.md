#  HTB Sherlock: Campfire-2
 * **Platform:** Hack The Box

* **Category:** DFIR

* **Difficulty:** Easy

* **Focus:** Windows Event Log Analysis

* **Tools:** Windows Event Viewer

## Senario
Investigate a suspicious Kerberos ticket request involving an unused administrator account and determine whether it indicates AS-REP Roasting.

## Investigation
- **Artifact:** 'Security.evtx' - Domain Controller Security Log.
- ""Objective:** Identify suspicoius Kerberos authentication activity and correlate related events.
- **Key Event ID:** '4768' - Kerberos Ticket Granting (TGT) request.
- **Detection indicator:** 'PreAuthType = 0 , which can indicate a request for an account without Kerberos pre-authentication.

## Findings
