# LedgerFlow Final | AI Development Prompt Log

**Project:** IS 3060 WOC Accounting Consulting Project  
**Prepared by:** Martel Steenblik  
**Final iteration:** November 24, 2026  
**AI tool:** ChatGPT  
**Live prototype:** [Launch LedgerFlow Final](https://bs-martel.github.io/IS-3060-WOC-Consulting-Project/Lab-7/LedgerFlow_Final.html#invoice-entry)

## 1. Purpose and development evidence

LedgerFlow began as a Lab 7 accounts payable prototype. For the final WOC consulting project, the existing application was extended to address missing receipt documentation and reconciliation exceptions identified through the Lab 2 accounting dataset. Of 600 expense records, 150 (25%) lacked receipts. The unmatched rate was 61.3% (92/150) without receipts versus 11.1% (50/450) with receipts. This comparison is an association, not proof of causation or financial loss.

The first three entries below summarize the build specifications recorded in my Lab 7 report. That report explicitly distinguishes these specifications from separate student-typed messages. The final iteration records actual student requests from the November 24 development conversation. This log is a curated development record, not a complete verbatim chat transcript.

## 2. Original Lab 7 iterations

### Iteration 1: As-is process
- **Documented build specification (summary):** Create a responsive, single-page HTML, CSS, Bootstrap and client-side JavaScript website for a small-business accounts payable department. Explain invoice intake, approval and payment using a basic workflow and sample information.
- **AI output:** A process overview and noninteractive sample invoice status table.
- **Reason for next iteration:** A static page described the process but could not capture or search live records.
- **Evidence:** [index_v1.html](index_v1.html), [Prompt 1 screenshot](Prompt%201%20index_v1.html_SS.png), [Lab 7 report](Lab7_Report_Martel_Steenblik.pdf).

### Iteration 2: Improved process
- **Documented build specification (summary):** Preserve the first draft and add a structured intake form with required-field and positive-amount validation, plus a searchable status tracker that updates when records are submitted.
- **AI output:** A validated form, browser-local records, updated counts and instant search.
- **Reason for next iteration:** Accounting staff needed better visibility into priorities, approval decisions and duplicate records.
- **Evidence:** [index_v2.html](index_v2.html), [Prompt 2 screenshot](Prompt%202%20index_v2.html_SS.png).

### Iteration 3: Innovative process
- **Documented build specification (summary):** Extend the existing client-side application with a dashboard, due-date alerts, manager review actions, local decision history, duplicate supplier/invoice checks and CSV export. Preserve intake, search and responsive layout.
- **AI output:** An interactive workflow covering Awaiting review, Approved, Needs correction and Paid, alongside decision-support and export features.
- **Reason for next iteration:** The WOC final project required a stronger connection to expense evidence and reconciliation, not just invoice approval.
- **Evidence:** [index_v3.html](index_v3.html), [Prompt 3 screenshot](Prompt%203%20index_v3.html_SS.png).

## 3. Final WOC-specific iteration: November 24, 2026

### Student request: Reuse the existing application
> well i have a lab 7 ledger flow we created couldnt that work?

**Development decision:** Build on the existing Lab 7 application instead of starting a separate prototype. Preserve the earlier HTML versions as evidence of iteration.

### Student request: Align the system to the receipt problem
> well we have to tie the recipts into the ledgerflow couldnt it be a better stratagie to highlight the existing problems with recipts and to instead use our new sytem ledger flow and show them hey this is a better way of tracking and do all out governance and cybersecurity based off that

**Development decision:** Connect the Tableau findings to receipt capture, missing-evidence exceptions, controlled approvals and reconciliation visibility. Explain production security and governance separately from working classroom controls.

### Student request: Produce the final version
> can you update the ledger flow to version 4 but call it just the final version of ledger flow

**AI output:** [LedgerFlow_Final.html](LedgerFlow_Final.html), a standalone browser-based application with:

- Shared intake for employee expenses and supplier invoices.
- Receipt or invoice attachments (PDF, JPG or PNG; maximum 500 KB per file).
- Missing-document flags and approval restrictions until evidence is attached.
- Duplicate checks, search, exception filters, transaction metrics and CSV export.
- Human approval, simulated payment and manual reconciliation using an external reference and matching amount.
- Local activity history and a description of proposed production safeguards.

### Student request: Prepare a demonstration artifact
> create a fake receipt that i can use as an example for when im demonstarting it in class

**AI output:** [LedgerFlow_Sample_Receipt.pdf](LedgerFlow_Sample_Receipt.pdf), a fictional classroom receipt from Summit Demo Office Supply (DEMO-1042, $128.40).

## 4. Demonstration and acceptance checks

The live GitHub Pages application URL was confirmed to open by the student. The following checks are the planned acceptance criteria for the live demo; individual results are not claimed as independently verified by this log.

| Step | Test | Expected outcome |
|---|---|---|
| 1 | Submit a fictional $128.40 employee expense without evidence. | Record appears with a missing-evidence flag. |
| 2 | Attempt approval before attaching the receipt. | Approval is blocked. |
| 3 | Attach the sample receipt and approve as a reviewer. | Missing-evidence flag clears and status advances to Approved. |
| 4 | Record simulated payment. | Status becomes Paid; reconciliation remains outstanding. |
| 5 | Enter a fictional external reference and matching amount. | Paid record becomes reconciled. |
| 6 | Attempt to create a duplicate transaction or reconcile using an incorrect amount. | Application rejects the inconsistent action. |

## 5. Governance, limitations and next steps

The prototype implements browser-side workflow logic, not production accounting infrastructure. It has no real authentication, server, bank connection or actual payments. Browser-local storage and activity history are not secure or tamper-proof. Attaching a document establishes its presence, not its authenticity. Use only fictional data.

Before any real deployment, WOC would need role-based access, MFA, segregation of duties, encrypted storage and transport, upload scanning, protected audit logs, backups, retention rules and testing. AI-assisted exception drafting is a proposed future feature; no AI approval, payment or reconciliation is implemented.

## 6. Repository evidence

- [Lab 7 folder and version history](https://github.com/BS-Martel/IS-3060-WOC-Consulting-Project/tree/main/Lab-7)
- [Live LedgerFlow Final](https://bs-martel.github.io/IS-3060-WOC-Consulting-Project/Lab-7/LedgerFlow_Final.html#invoice-entry)
- [Original Lab 7 report](Lab7_Report_Martel_Steenblik.pdf)
- [Fictional demonstration receipt](LedgerFlow_Sample_Receipt.pdf)

The earlier build specifications and screenshots are retained as evidence of development; the final student requests document the WOC-specific iteration. The prototype supports the proposed consulting solution but does not demonstrate actual savings or verified production security.
