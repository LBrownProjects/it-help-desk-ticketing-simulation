# Simulated Help-Desk Tickets

This document records incidents completed as part of a guided learning simulation for the fictional clinic **Palmetto DentalWorks**. All people, systems, incidents, and results are fictional.

## Progress

- [x] Ticket 001: Locked DentalRecord account
- [x] Ticket 002: Workstation Print Queue Failure
- [ ] Ticket 003
- [ ] Ticket 004
- [ ] Ticket 005

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
