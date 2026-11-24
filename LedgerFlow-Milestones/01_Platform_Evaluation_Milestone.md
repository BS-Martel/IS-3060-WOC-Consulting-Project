# LedgerFlow | Technology and Platform Evaluation

**IS 3060-004 · WOC Accounting Consulting Project · November 24, 2026**  
**Rubric alignment:** Milestone 5 / Slide 7  
**Status:** Supplemental final-project evaluation, not a previously submitted milestone.

## Decision to make

WOC needs a consistent way to capture expense evidence, review exceptions, approve transactions and track reconciliation. The Lab 2 workbook contains 600 expenses: 150 (25%) lack receipts, and 142 (23.7%) are unmatched. The unmatched rate is 61.3% without receipts versus 11.1% with receipts. These findings support prioritizing documentation controls; they do not establish causation or financial loss.

The recommendation is to pilot the LedgerFlow workflow using fictional data, then evaluate a secure production platform before processing real financial information. The goal is not to deploy the public browser prototype as a financial system.

## Comparison of alternatives

| Alternative | Fit and business value | Cost considerations | Scalability | Principal risk |
| --- | --- | --- | --- | --- |
| Manual process / spreadsheets | Familiar; basic expense tracking; weak shared evidence and exception visibility | Low initial technology cost; recurring staff time and rework | Limited by manual review and version coordination | Missing or duplicate records; inconsistent controls |
| Thunkable intake concept (Lab 3) | Structured mobile submission and receipt reminders; useful for front-end intake | Low-code build effort; licensing, storage and integration costs to confirm | Potentially useful across departments; verify limits and integrations | Access permissions, attachment storage and integration with accounting |
| LedgerFlow Final (Lab 7 evolution) | Strong workflow fit: intake, evidence flags, approval gate, duplicate checks, simulated payment and manual reconciliation | Existing classroom prototype; production engineering, hosting, maintenance and training would require funding | Browser demo is suitable for classroom validation only; shared database and backend required for scale | No production authentication, centralized records or protected audit logs |
| Secure accounting platform (commercial or custom) | Potential end-to-end workflow with shared records, approvals, audit and integrations; verify actual feature fit | Subscription or development cost, migration, configuration, training, support and exit costs | Potentially strong if capacity, availability and integrations are verified | Vendor dependency, migration and configuration risk |

These are qualitative judgments, not vendor quotations or procurement results. WOC's budget, current accounting stack and transaction volumes beyond the class dataset are unknown. No specific vendor or licensing tier is assumed.

## Evaluation criteria and decision method

Use the following proposed weights when evaluating real production candidates. Score each candidate from 1 (poor) to 5 (strong) after demonstrations, security review and cost estimates. The total weighted score is the sum of each rating multiplied by its weight, divided by 5, expressed out of 100. Do not score missing evidence as a confirmed capability.

| Criterion | Weight | Evidence required |
| --- | ---: | --- |
| Accounting workflow fit | 35% | Demonstrate receipt submission, exception queue, approval separation and reconciliation |
| Security and governance risk | 30% | Verify MFA, role permissions, protected audit trail, encryption, backup and retention |
| Total cost of ownership | 20% | Written estimates for implementation, licensing, integration, training, maintenance and exit |
| Scalability and integration | 15% | Multi-user tests, data export, accounting integration and performance at expected volumes |

**Mandatory security gate:** No production candidate advances solely because it scores well. It must pass access, data protection, audit, recovery and segregation-of-duties checks. A browser-only demo cannot meet this gate without substantial redevelopment.

## Cost and feasibility validation

- Compare three-year costs: setup + migration + integration + training + recurring subscriptions or hosting + support + contingency. Obtain written estimates before choosing build versus buy.
- Estimate staff time saved from measured review minutes per transaction and exception volume; do not claim savings before a pilot establishes a baseline.
- Retain Tableau for management analysis if integration and data access are approved. Avoid replacing working accounting systems merely to demonstrate a new tool.
- Prefer configuring a secure existing platform if it meets the workflow and control requirements at a reasonable cost. Consider custom development only when gaps justify the ongoing support obligation.

## Recommendation and next steps

1. Demonstrate LedgerFlow Final with fictional records; gather feedback from accounting and department users.
2. Confirm workflow needs, existing systems, budget and security requirements.
3. Test production candidates using the same receipt, approval and reconciliation scenarios.
4. Compare verified costs and weighted criteria; select a platform only after security approval.
5. Run a limited pilot and expand only if the measured results justify the investment.

## Evidence

- [Lab 2 Tableau analysis](../Lab-2/)
- [Lab 3 Thunkable concept](../Lab-3/)
- [Lab 7 LedgerFlow prototype and development history](../Lab-7/)
- [Lab 10 AI strategy and sourcing coursework](../Lab-10/): transferable evaluation approach, not a WOC vendor assessment.
- [Live LedgerFlow classroom prototype](https://bs-martel.github.io/IS-3060-WOC-Consulting-Project/Lab-7/LedgerFlow_Final.html#invoice-entry)
- [Risk register](03_Cybersecurity_Risk_Register.md) and [implementation roadmap](04_Implementation_Roadmap.md)
