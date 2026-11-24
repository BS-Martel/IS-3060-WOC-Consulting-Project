# WOC Accounting Process Improvement | IS 3060 Consulting Project

**Course:** IS 3060-004, Fall 2026, University of Utah  
**Selected group focus:** Accounting Track  
**Original lab work contributed by:** Martel Steenblik  
**Project context:** WOC expense documentation, reconciliation, and accounting process improvement

## The business problem

WOC's accounting dataset highlights a documentation and reconciliation issue. In the 600-expense dataset analyzed in Lab 2, 150 transactions lacked an attached receipt. Of those 150, 92 were unmatched (61.3%). By comparison, 50 of the 450 transactions with an attached receipt were unmatched (11.1%). Expenses without receipts accounted for $118,620.44 of the $179,361.87 in unmatched spending.

These descriptive results do **not** demonstrate that missing receipts caused every reconciliation failure. They support prioritizing stronger receipt documentation, better exception visibility, and a more consistent review process.

## Consulting recommendation

Use a phased approach to improve accounting accuracy and visibility:

1. **Standardize expense intake.** Capture employee, department, amount, and category in a consistent form, and prompt users to provide supporting receipts.
2. **Improve exception monitoring.** Use dashboard views to identify missing receipts, unmatched transactions, and pending reconciliations.
3. **Streamline review workflows.** Evaluate digital invoice intake, required-field checks, duplicate detection, approval/status tracking, and audit records. The Lab 7 prototype shows these ideas for accounts payable, a related but distinct accounting process.
4. **Evaluate automation responsibly.** Treat AI-assisted analysis as an opportunity to test, not as an already-deployed WOC system. Verify outputs, keep employees in control of approvals, and review security, privacy, cost, and sourcing before implementation.

## Original lab coursework and evidence

The files below are the **original coursework artifacts** created across the semester, organized for the final consulting review. PDF copies of Word submissions are provided for convenient browser viewing. The connection notes in the lab folders explain how the original work informs this accounting recommendation.

| Lab | Original work and evidence | Role in the consulting recommendation |
| --- | --- | --- |
| [Lab 2: Tableau](Lab-2/) | Superstore and WOC Tableau packaged workbooks (`.twbx`), original reflection and WOC consulting memo | Evidence of receipt and reconciliation exceptions; basis for management dashboard recommendations |
| [Lab 3: Thunkable](Lab-3/) | Employee-directory and WOC expense-submission app screenshots, app links, reflection and memo | Illustrates structured digital expense intake and a receipt reminder |
| [Lab 7: LedgerFlow](Lab-7/) | Three original HTML versions, final LedgerFlow prototype, prompt log, screenshots, and report | Demonstrates a related accounts-payable process improving through validation, duplicate controls, approval steps, and status visibility |
| [Lab 8: AI Assistant](Lab-8/) | Denver Broncos AI assistant report with four tested social-media scenarios | Transferable demonstration of structured AI inputs, knowledge grounding, human review, and test limitations, **not** an accounting bot deployed at WOC |
| [Lab 10: AI Sourcing](Lab-10/) | Decathlon image-classification pilot and outsourcing proposal, model/test screenshots, candidate review | Transferable method for evaluating AI feasibility, weak evidence, governance, pilot costs, and build-versus-outsource decisions, **not** a WOC-trained model |

## LedgerFlow final prototype

[**Launch LedgerFlow Final**](https://bs-martel.github.io/IS-3060-WOC-Consulting-Project/Lab-7/LedgerFlow_Final.html#invoice-entry)

The final classroom prototype extends the three Lab 7 versions to address WOC's receipt documentation and reconciliation problem. It demonstrates receipt attachments, missing-evidence approval restrictions, duplicate checks, human approval, simulated payment and manual reconciliation. It uses browser-local demo records, not a secure production backend.

- [Final prototype source](Lab-7/LedgerFlow_Final.html)
- [AI development prompt log](Lab-7/AI_Prompt_Log.md)
- [Fictional demonstration receipt](Lab-7/LedgerFlow_Sample_Receipt.pdf)

## LedgerFlow supporting documentation

These documents consolidate original coursework and supplemental analysis finalized for the executive presentation.

| Document | Presentation connection |
| --- | --- |
| [Technology and Platform Evaluation](LedgerFlow-Supporting-Documentation/01_Platform_Evaluation.md) | Slide 7: technology fit, cost, scalability and risk |
| [Accounting Process Map](LedgerFlow-Supporting-Documentation/02_Accounting_Process_Map.md) | Slides 5–6: current and future accounting workflows |
| [Cybersecurity Risk Register](LedgerFlow-Supporting-Documentation/03_Cybersecurity_Risk_Register.md) | Slide 9: risks and proposed controls |
| [Implementation Roadmap](LedgerFlow-Supporting-Documentation/04_Implementation_Roadmap.md) | Slide 11: 2027 rollout, responsibilities and measurable goals |

See the [supporting documentation index](LedgerFlow-Supporting-Documentation/README.md) for the full evidence map. The roadmap proposes raising receipt attachment from 75% to 95%, reducing unmatched transactions from 23.7% to 12%, and reaching a median approval turnaround of two business days by December 2027. These are proposed targets, not achieved results; the approval-time baseline is not yet measured.

## How to examine the evidence

- **Tableau:** Open the `.twbx` files in a compatible Tableau application. The packaged WOC workbook includes the dataset used in Lab 2.
- **Lab 3 prototypes:** The original report includes screenshots and links for both Thunkable apps. [Employee directory app](https://x.thunkable.com/copy/c870a585cbaeea63d12d91d3278af2c7) and [WOC expense app](https://x.thunkable.com/copy/ba8e235886848dbbaad060671a6dae5b).
- **Lab 7 interactive prototype:** Launch LedgerFlow Final using the link above, or download and open `Lab-7/LedgerFlow_Final.html` in a browser. The three original versions document iteration. The prototype uses browser-side sample data, not a production accounting database or authenticated service.
- **Documents:** The PDF versions can be viewed directly on GitHub; the original `.docx` documents are preserved alongside them.
- **AI lab evidence:** Read Lab 8 and Lab 10 as evidence of learning and methodology; neither original lab was designed for the WOC accounting case.

## Evidence and scope

This repository compiles completed individual lab submissions into a single project navigation structure. The project proposal and recommendations above are educational, not documentation of deployed systems. The original Lab 7 accounts-payable demonstration informed the final WOC-specific expense and reconciliation prototype. Suggested AI applications would require new WOC-specific design, validation, and approval before adoption.

To support the final group presentation, the team should explain how these artifacts fit together, identify the highest-priority WOC control issue, and distinguish observed data from planned improvements.
