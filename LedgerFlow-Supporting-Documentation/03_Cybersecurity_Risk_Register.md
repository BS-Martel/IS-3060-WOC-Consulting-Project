# LedgerFlow | Cybersecurity, Privacy and Governance Risk Register

**IS 3060-004 · WOC Accounting Consulting Project · November 24, 2026**  
**Rubric alignment:** Milestone 9 / Slide 9  
**Status:** Supplemental proposed risk register. Ratings are qualitative planning judgments, not measured incident frequencies or a formal WOC security assessment.

## Scope

LedgerFlow Final is a public GitHub Pages classroom prototype that uses browser-local storage, evidence uploads, workflow checks, simulated payments and manual matching. It is not authorized for real receipts, personal data, bank records or payment processing. Real use requires a secure production system with authenticated access and centralized controls. AI-assisted exception follow-up is a proposed future feature, not an integrated capability.

## Rating method

Likelihood: Low = unlikely under assumed conditions; Medium = plausible; High = expected or frequent without safeguards. Impact: Low = limited disruption; Medium = material rework or operational disruption; High = potential financial misstatement, privacy breach, loss of evidence or substantial disruption. Assign Low/Medium/High numeric values of 1/2/3 and multiply for prioritization. Scores 1–2 are Low, 3–4 Medium, 6–9 High. Ratings below describe inherent risk in a future deployment before the recommended controls; validate against WOC's actual environment.

## Priority risks

| ID | Risk and business impact | Likelihood | Impact | Priority | Recommended controls | Accountable role (proposed) |
| --- | --- | --- | --- | --- | --- | --- |
| R1 | Unauthorized access or approval: someone views sensitive records or approves their own expense | Medium | High | High (6) | MFA; least-privilege role-based access; separate submitter, approver and payment roles; revoke access when staff leave | IT/security + finance lead |
| R2 | Receipt data exposure or malicious file upload: financial or personal information is disclosed, or a file compromises systems | Medium | High | High (6) | Encrypted transport and storage; private file storage; file type/size limits and malware scanning; approved retention and deletion policy | IT/security |
| R3 | Incorrect AI output: fabricated evidence, wrong amount or unauthorized instruction leads to an erroneous decision | Medium | High | High (6) | Limit AI to drafting and flagging; ground outputs in authorized records; human review; no approval, payment or reconciliation permissions; test failure cases | Accounting lead + IT |
| R4 | Duplicate or altered records: duplicate payment or manipulated evidence compromises financial reporting | Medium | High | High (6) | Server-side uniqueness and validation; approval history; tamper-resistant audit logs; reconcile against independent records | Accounting lead + IT |
| R5 | Loss of transaction records or attachments: device failure or deletion removes financial evidence | Medium | High | High (6) | Centralized protected storage; automated backups; tested restores; recovery responsibilities | IT |
| R6 | Deployment or integration failure: transactions are incomplete, duplicated or incorrectly posted across systems | Medium | High | High (6) | Test integrations on fictional records; reconcile control totals; phased migration; rollback plan and exception monitoring | IT + accounting |

R1–R4 align directly with the four risks on Slide 9. R5–R6 supplement the deployment plan. No residual risk rating is claimed until controls have been implemented and tested.

## Existing demonstration controls versus production requirements

| Demonstrated in LedgerFlow Final | Required before real deployment |
| --- | --- |
| Missing-evidence flag and approval restriction | Server-side validation, authentic evidence checks and documented exception policy |
| Duplicate detection and ordered status changes | Database uniqueness, transactional integrity and authenticated approvals |
| Local activity history | Centralized, access-controlled audit logs with protected retention |
| Attachment type/size restrictions | Server-side scanning, encrypted private storage and authorized access |
| Simulated payment and manual matching | Approved accounting-system integration; segregation of duties; verified external references |

Browser-side checks can be bypassed and local data can be altered or lost. No real MFA, secure multi-user authorization, protected audit trail, bank integration or AI controls are currently implemented.

## Pre-production acceptance checks

| Test | Required outcome before real use |
| --- | --- |
| Submitter tries to approve own transaction | Server refuses; event logged |
| Unauthorized user tries to access another department's restricted receipt | Access denied; event logged |
| Missing receipt or duplicate transaction | Approval blocked or routed for authorized investigation; no payment triggered |
| Disallowed or malicious test attachment | Upload rejected or quarantined; no user exposure |
| Restore records from a test backup | Records, attachments and audit history restored and reconciled |
| AI asked to fabricate evidence or bypass approval | Refuses, flags exception and routes to a human; no financial action |

These are proposed production acceptance criteria, not completed tests. Use synthetic fixtures in a controlled environment. See [Lab 8 supplemental scenarios](../Lab-8/LedgerFlow_AI_Exception_Tests.md) if uploaded.

## Governance and incident response

- Finance defines receipt and approval policy; IT implements and reviews permissions. If staffing prevents full segregation, require independent review and documented compensating controls.
- Minimize data collection, restrict exports, and set retention in line with WOC's confirmed obligations; avoid claiming a specific legal retention period without review.
- Require human approval of AI-generated messages and review exception trends. Never send sensitive receipt information to an unapproved AI service.
- Review access and risk controls quarterly and after major changes. If a suspected incident occurs, suspend affected workflows, preserve logs, notify finance and IT, investigate, recover and reconcile before restarting.
- Begin with existing approved identity, storage and backup services where feasible; validate budget and procurement before adding vendors.

## Evidence

- [Lab 7 prototype](../Lab-7/) and [live demo](https://bs-martel.github.io/IS-3060-WOC-Consulting-Project/Lab-7/LedgerFlow_Final.html#invoice-entry)
- [Lab 8 AI coursework](../Lab-8/) and [Lab 2 analysis](../Lab-2/)
- [Platform evaluation](01_Platform_Evaluation.md) and [roadmap](04_Implementation_Roadmap.md)
