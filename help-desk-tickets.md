# Simulated Help-Desk Tickets

This document records incidents completed as part of a guided learning simulation for the fictional clinic **Palmetto DentalWorks**. All people, systems, incidents, and results are fictional.

## Progress

- [x] Ticket 001: Locked DentalRecord account
- [x] Ticket 002: Workstation Print Queue Failure
- [x] Ticket 003: VPN Failure After Windows Update
- [x] Ticket 004: Credential-Phishing Incident
- [x] Ticket 005: OneDrive File Sync Failure

## Ticket 001: Locked DentalRecord Account

| Field | Details |
| --- | --- |
| Ticket ID | PWH-INC-001 |
| Requester | Jessi Smith, Front Desk |
| Category | Identity and Access Management |
| Priority | P3 - Medium |
| Status | Resolved |
| Escalated | No |

### Issue Description

Jessi reported being unable to sign in to DentalRecord after several unsuccessful attempts. Patients were beginning to arrive, but another receptionist could continue checking them in.

### Business Impact

One employee was unable to access the patient check-in system. Clinic operations continued using another receptionist, although the front desk was beginning to experience delays. Because one user was affected and a temporary workaround existed, the ticket was assigned P3 - Medium priority.

### Troubleshooting Performed

1. Asked Jessi for the exact error message to narrow down the problem.
2. Confirmed that the message identified an account lockout.
3. Verified Jessi's identity using the clinic's approved procedure.
4. Checked the account status and recent sign-in activity.
5. Confirmed that the account was active but locked.
6. Confirmed that the failed attempts came from Jessi's usual clinic computer.
7. Found no signs of suspicious or unauthorized access.
8. Learned that Jessi had accidentally entered an old password.
9. Unlocked the account and asked Jessi to sign in using the recently created password.
10. Confirmed that Jessi could access DentalRecord and open the patient check-in screen.

### Resolution

Jessi's existing account was unlocked. Jessi successfully signed in with the correct password and confirmed that normal DentalRecord access was restored.

### Closure Note

The resolution was documented, the requester confirmed that service was restored, and the ticket was closed.


## Ticket 002: Workstation Print Queue Failure

| Field | Details |
| --- | --- |
| Ticket ID | PWH-INC-002 |
| Requester | Jasmine Jefferson, Billing |
| Category | Hardware and Printing |
| Priority | P3 - Medium |
| Status | Resolved |
| Escalated | No |

### Issue Description

Jasmine reported that the billing printer appeared offline. She submitted two documents, but neither printed. The documents were required for the day's billing work.

### Business Impact

One billing employee was unable to print from her workstation. Other employees could continue printing, and an alternate workstation or printer was available. The issue created a same-day work delay but did not stop clinic operations. Because the impact was limited but the work had same-day urgency, the ticket was assigned P3 - Medium priority.

### Troubleshooting Performed

1. Asked whether other billing employees could print to determine the scope of the incident.
2. Confirmed that two coworkers could print successfully.
3. Determined that the printer had power, was connected to the network, and was available to other users.
4. Verified that Jasmine selected the correct network printer.
5. Inspected Jasmine's print queue and found two jobs with the status "Error - Printing."
6. Canceled the stalled print jobs.
7. Restarted the Windows Print Spooler service using the approved procedure.
8. Printed an approved, non-sensitive test page.
9. Asked Jasmine to resubmit one billing document.
10. Confirmed that the billing document printed successfully.

### Resolution

Two stalled jobs were removed from Jasmine's print queue, and the Windows Print Spooler service was restarted. The test page and Jasmine's billing document printed successfully.

### Closure Note

Jasmine confirmed that normal printing was restored. She was reminded to retrieve sensitive documents promptly. The troubleshooting steps and resolution were documented, and the ticket was closed.

### Escalation Decision

The ticket was not escalated because the printer remained available to other employees and routine Tier 1 troubleshooting resolved the workstation-specific problem.


### Escalation Decision

The incident was not escalated because it fell within Tier 1 authority, the requester's identity was verified, no suspicious activity was present, and the standard account-unlock procedure resolved the problem.


## Ticket 003: VPN Failure After Windows Update

| Field | Details |
| --- | --- |
| Ticket ID | PWH-INC-003 |
| Requester | Ashley Brown, Practice Administration |
| Category | Network and Remote Access |
| Priority | P2 - High |
| Status | Resolved |
| Escalated | Yes - Tier 2 Network Support |

### Issue Description

Ashley reported being unable to establish a secure VPN connection while working remotely. General internet access and Microsoft Outlook continued working. The VPN had worked the previous day, but Ashley's clinic laptop installed a Windows update overnight.

### Business Impact

Ashley could not access internal clinic resources needed for a time-sensitive business deadline. No approved alternative method of accessing or transferring the files was available.

### Troubleshooting Performed

1. Confirmed that Ashley had general internet access.
2. Recorded the exact VPN error: "A secure connection could not be established."
3. Checked for a wider VPN outage and confirmed that the VPN service was operational.
4. Confirmed that Ashley's account was active and not locked.
5. Restarted the VPN application.
6. Restarted the clinic laptop.
7. Verified that Ashley selected the approved VPN profile.
8. Confirmed that the VPN client was current.
9. Retried the connection and received the same error.
10. Collected the permitted VPN diagnostic logs.
11. Escalated the incident to Tier 2 Network Support with the error, business impact, recent update, logs, and completed troubleshooting steps.

### Tier 2 Action

Tier 2 determined that the Windows update had disrupted the VPN's virtual network-adapter component. The technician, Cam Bethea, repaired the approved component and restored the VPN connection.

### Resolution

Ashley successfully connected to the VPN and accessed the required internal clinic resources.

### Closure Note

Ashley confirmed that normal access was restored. Tier 1 documented the troubleshooting, escalation, Tier 2 repair, and user confirmation before closing the ticket.

### Escalation Decision

The incident required escalation because authorized Tier 1 troubleshooting did not resolve the failure and repair of the VPN network component required Tier 2 access and expertise.

### Priority Decision

This incident was classified P2 - High because essential, time-sensitive work was blocked, no approved workaround was available, and specialized support was required. It was not P1 because the VPN service remained available to other employees and the clinic was not experiencing a widespread outage.



## Ticket 004: Credential-Phishing Incident

| Field | Details |
| --- | --- |
| Ticket ID | PWH-SEC-004 |
| Requester | Nisha Phillips, Medical Assistant |
| Category | Information Security |
| Priority | P1 - Critical |
| Status | Resolved |
| Escalated | Yes - Information Security |
| Assigned analyst | Mason Israel, Information Security Analyst |

### Issue Description

Nisha received an email that appeared to come from Microsoft. It warned that her clinic account would be disabled unless she verified it immediately. Nisha selected the link and entered her clinic email address and password. She denied the unexpected MFA request, closed the website, and contacted the help desk.

### Business and Security Impact

Nisha's password was exposed to a malicious website. The attacker attempted to complete the sign-in using MFA, and similar messages were present in other clinic mailboxes. The incident created a risk of unauthorized access to clinic systems and protected information.

### Initial Response

1. Instructed Nisha not to interact further with the email or website.
2. Asked whether she entered credentials, approved MFA, downloaded a file, or opened an attachment.
3. Confirmed that Nisha entered her email address and password.
4. Confirmed that she denied the MFA prompt.
5. Confirmed that she did not download a file or open an attachment.
6. Preserved the original email using the clinic's approved reporting procedure.
7. Immediately escalated the incident to Information Security.
8. Initiated the clinic's approved compromised-account response process.

### Information Security Response

Mason Israel, Information Security Analyst:

1. Directed the approved password-reset process.
2. Revoked Nisha's existing account sessions.
3. Reviewed recent sign-in activity.
4. Confirmed that no unauthorized sign-in succeeded.
5. Blocked the malicious sender and website.
6. Removed matching phishing emails from other clinic mailboxes.

### Resolution

Nisha created a new password through the clinic's official process and successfully signed in using the new password and MFA. Information Security confirmed that the attempted compromise was contained.

### Closure Note

Nisha confirmed normal account access. The security team's findings and containment actions were documented according to clinic policy. Nisha received guidance about suspicious urgency, credential requests, unexpected MFA prompts, and approved phishing-reporting procedures.

### Escalation Decision

The incident was escalated immediately because exposed credentials, an unauthorized MFA attempt, and similar messages in other mailboxes required security tools and authority beyond Tier 1.

### Priority Decision

The incident was assigned P1 - Critical because it presented a potentially widespread security threat and risk of unauthorized access to protected clinic information. Immediate containment was required even though the MFA denial prevented a successful sign-in.

## Ticket 005: OneDrive File Sync Failure

**Ticket ID:** PWH-INC-005 
**Requester:** Danielle Brooks 
**Department:** Billing 
**Category:** Software / Microsoft 365 / OneDrive 
**Priority:** P3 
**Status:** Resolved 
**Escalated:** No 

### Issue Description

Danielle reported that the file `Daily Billing: Reconciliation?.xlsx` was not syncing through Microsoft OneDrive. A red X appeared beside the file, preventing her from accessing the current version from the shared workstation.

### Business Impact

The issue affected one employee and delayed Danielle's ability to complete the daily billing reconciliation. No data was lost, and the clinic remained operational.

### Troubleshooting Performed

1. Confirmed that Danielle was signed in to the correct Microsoft 365 account.
2. Identified the affected file in the OneDrive folder.
3. Reviewed the OneDrive sync-status message.
4. Determined that the colon and question mark in the filename were unsupported characters.
5. Renamed the file to `Daily Billing Reconciliation.xlsx`.
6. Allowed OneDrive to resume syncing.
7. Confirmed that the red X disappeared.
8. Asked Danielle to open the file from the synced location and verify its contents.
9. Danielle confirmed that the file opened successfully and contained the current billing information.

### Resolution

Removed the unsupported characters from the filename. OneDrive successfully synced the renamed file, and Danielle regained access to the current version from the shared workstation.

### Closure Note

Danielle confirmed that she could open the current version of `Daily Billing Reconciliation.xlsx`. No additional problems were reported. The ticket was resolved and closed.

### Priority Decision

The ticket was assigned **P3 priority** because the issue affected one employee and one file. Work was temporarily delayed, but there was no data loss or organization-wide outage.

### Escalation Decision

The ticket was not escalated. Tier 1 identified the cause, completed the corrective action within its authority, and confirmed the resolution with the requester.
