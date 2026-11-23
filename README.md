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

## Milestone artifacts

The files below are the **original coursework artifacts** created across the semester, organized for the final consulting review. PDF copies of Word submissions are provided for convenient browser viewing. Each folder contains `CONNECTION_TO_WOC.md`, explaining how the original work informs this accounting recommendation.

| Lab | Original work and evidence | Role in the consulting recommendation |
| --- | --- | --- |
| [Lab 2: Tableau](Lab-2/) | Superstore and WOC Tableau packaged workbooks (`.twbx`), original reflection and WOC consulting memo | Evidence of receipt and reconciliation exceptions; basis for management dashboard recommendations |
| [Lab 3: Thunkable](Lab-3/) | Employee-directory and WOC expense-submission app screenshots, app links, reflection and memo | Illustrates structured digital expense intake and a receipt reminder |
| [Lab 7: LedgerFlow](Lab-7/) | Three runnable HTML website versions, screenshots, and report | Demonstrates a related accounts-payable process improving through validation, duplicate controls, approval steps, and status visibility |
| [Lab 8: AI Assistant](Lab-8/) | Denver Broncos AI assistant report with four tested social-media scenarios | Transferable demonstration of structured AI inputs, knowledge grounding, human review, and test limitations, **not** an accounting bot deployed at WOC |
| [Lab 10: AI Sourcing](Lab-10/) | Decathlon image-classification pilot and outsourcing proposal, model/test screenshots, candidate review | Transferable method for evaluating AI feasibility, weak evidence, governance, pilot costs, and build-versus-outsource decisions, **not** a WOC-trained model |

## How to examine the evidence

- **Tableau:** Open the `.twbx` files in a compatible Tableau application. The packaged WOC workbook includes the dataset used in Lab 2.
- **Lab 3 prototypes:** The original report includes screenshots and links for both Thunkable apps. [Employee directory app](https://x.thunkable.com/copy/c870a585cbaeea63d12d91d3278af2c7) and [WOC expense app](https://x.thunkable.com/copy/ba8e235886848dbbaad060671a6dae5b).
- **Lab 7 interactive prototype:** Download and open `Lab-7/index_v3.html` in a browser. Drafts 1 and 2 are also included to document iteration. The prototype uses browser-side sample data, not a production accounting database or authenticated service.
- **Documents:** The PDF versions can be viewed directly on GitHub; the original `.docx` documents are preserved alongside them.
- **AI lab evidence:** Read Lab 8 and Lab 10 as evidence of learning and methodology; neither original lab was designed for the WOC accounting case.

## Evidence and scope

This repository compiles completed individual lab submissions into a single project navigation structure. The project proposal and recommendations above are educational, not documentation of deployed systems. The Lab 7 accounts-payable demonstration is related to, but separate from, the WOC employee-expense process. Suggested AI applications would require new WOC-specific design, validation, and approval before adoption.

To support the final group presentation, the team should explain how these artifacts fit together, identify the highest-priority WOC control issue, and distinguish observed data from planned improvements.
