**Summerville FCU**

**Web Check Deposit (Online Banking)**

Feature Guide | Platform: nFinia Online Banking | Prepared by: Jeeva PM
| April 2026

**1. PRODUCT SUMMARY**

Web Check Deposit on Summerville FCU's nFinia platform enables business
You to deposit checks from any web browser — no mobile device or
branch visit required. You upload front and back check images via a
drag-and-drop or file-upload interface, with the system displaying
real-time account details including current balance and deposit limit.

The feature offers a dual-tab interface: the "Deposit Your Check" tab
for submitting new deposits, and the "Check Deposit History" tab for
tracking all deposits across every channel — Online, Mobile, Branch, and
ATM. This cross-channel history view is especially valuable for business
You managing multiple deposit channels.

For Summerville FCU, web check deposit extends RDC access to You who
prefer desktop banking, provides a high deposit limit ($30,000 shown),
and creates a complete multi-channel audit trail for BSA/AML and Reg CC
compliance.

**At-a-Glance**

|                      |                                                                                      |
| -------------------- | ------------------------------------------------------------------------------------ |
| **Attribute**        | **Detail**                                                                           |
| Feature Name         | Web Check Deposit (Remote Deposit Capture via Online Banking)                        |
| Module               | Accounts > Check Deposit                                                            |
| User Roles           | Business Member (online banking), Operations Staff                                   |
| Access Level         | Requires RDC enrollment and valid account                                            |
| Key Actions          | Select account, upload front/back images, submit; view history                       |
| Regulatory Relevance | Reg CC (funds availability), BSA/AML (deposit monitoring), multi-channel audit trail |

**2. USE CASES**

|                              |                             |                                                                                                                               |                                                                            |
| ---------------------------- | --------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| **Use Case**                 | **Who Uses It**             | **What They Do**                                                                                                              | **Business Value**                                                         |
| New Check Deposit            | Business member             | Selects account, reviews balance and deposit limit, uploads front and back check images via drag-drop or file picker, submits | Enables deposit from any computer; no scanner or branch visit required     |
| Deposit Limit Review         | Finance manager             | Views displayed deposit limit before entering amount to avoid rejection                                                       | Prevents rejected deposits; sets clear member expectations                 |
| Historical Lookup            | Operations / Compliance     | Filters deposit history by date range and account; views receipt numbers and status                                           | Supports audit trail; enables BSA/AML monitoring                           |
| Multi-Channel Reconciliation | Accountant                  | Views deposits from Online, Mobile, Branch, and ATM channels in one unified history view                                      | Simplifies reconciliation; single source of truth for all deposit channels |
| Check Image Retrieval        | Member / Compliance officer | Clicks View Image in history to see front and back thumbnails of a previously deposited check                                 | Supports dispute resolution, member inquiries, and compliance review       |

**3. END-TO-END WORKFLOW**

**3.1 Prerequisites**

• RDC enrollment active on you account

• Account eligible for web check deposit (configured by Summerville FCU)

• Modern web browser; check images as JPG or PNG files ready to upload

**3.2 Step-by-Step Flow**

|          |                                                                         |                                                                                                        |
| -------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| **Step** | **Action**                                                              | **System Response**                                                                                    |
| 1        | Log in to online banking; navigate to Accounts > Check Deposit         | "Deposit Your Check" tab displayed by default                                                          |
| 2        | Select account from dropdown                                            | System displays: Account Number, Membership Number, Current Balance ($829.00), Deposit Limit ($30,000) |
| 3        | Enter Amount to Deposit                                                 | Field validates numeric input against displayed deposit limit                                          |
| 4        | Upload FRONT image: click upload area or drag-and-drop check image file | File selected; thumbnail preview shown in front upload area                                            |
| 5        | Upload BACK image: click upload area or drag-and-drop endorsed back     | File selected; thumbnail preview shown in back upload area                                             |
| 6        | Review entries; click "Deposit Check" button                            | System validates: amount vs. limit, file validity, account status                                      |
| 7        | Validation passes                                                       | Success confirmation with receipt number displayed                                                     |
| 8        | Click "Check Deposit History" tab                                       | History table shows new entry: Date, Amount, Receipt No., Channel (Online), Status (Submitted)         |

**3.3 Decision Points & Error Handling**

|                              |                                                                       |
| ---------------------------- | --------------------------------------------------------------------- |
| **Condition**                | **System Behavior**                                                   |
| Amount exceeds deposit limit | "Exceeds deposit limit" error; deposit blocked until amount corrected |
| Invalid file format uploaded | Error message: "Please upload a valid image file (JPG or PNG)"        |
| Account not eligible for RDC | Account not shown in account dropdown                                 |
| Clear button clicked         | All entered data cleared; form resets to initial state                |

**3.4 Completion**

Upon successful submission, a confirmation screen shows the receipt
number and deposit amount. The transaction immediately appears in the
Check Deposit History tab with status "Submitted" and channel "Online."
History records are retained for the configured retention period and are
available for compliance review.

**4. FEATURE OVERVIEW — UI WALKTHROUGH**

**Screen 1: Deposit Your Check**

<figure><img src="/.gitbook/assets/82f93319ebbf1b2e491e21b3f18ed1a5da2ff5c6.png" alt="" width="480"><figcaption></figcaption></figure>

*Figure 1: Web deposit form showing account details, balance, deposit
limit, and image upload areas*

|                      |                        |                                                                |
| -------------------- | ---------------------- | -------------------------------------------------------------- |
| **Field / Element**  | **Type**               | **Description**                                                |
| Account Name         | Dropdown               | Selects target deposit account; required                       |
| Account Number       | Display field          | Shows full account number after account selection              |
| Membership Number    | Display field          | Member ID associated with the selected account                 |
| Current Balance      | Display field          | Real-time account balance (e.g. $829.00)                       |
| Deposit Limit        | Display field          | Maximum deposit amount allowed for this account (e.g. $30,000) |
| Amount to Deposit    | Numeric input          | Dollar amount of the check; validated against deposit limit    |
| FRONT upload area    | File input / drag-drop | Click or drag-drop check front image (JPG/PNG)                 |
| BACK upload area     | File input / drag-drop | Click or drag-drop endorsed back image (JPG/PNG)               |
| Clear button         | Secondary action       | Resets all fields on the deposit form                          |
| Deposit Check button | Primary action         | Submits deposit after all fields are filled                    |

**Screen 2: Check Deposit History**

<figure><img src="/.gitbook/assets/8503f46ecf3dcc3560dee8c9763c77ae7e8fbb7e.png" alt="" width="620"><figcaption></figcaption></figure>

*Figure 2: History tab showing multi-channel deposit records with filter
options and view image capability*

|                           |                         |                                                                         |
| ------------------------- | ----------------------- | ----------------------------------------------------------------------- |
| **Field / Element**       | **Type**                | **Description**                                                         |
| Deposit Your Check tab    | Navigation tab          | Switches to the new deposit submission form                             |
| Check Deposit History tab | Navigation tab (active) | Shows all deposit history across all channels                           |
| Date From / Date To       | Date filter             | Filters history records by date range                                   |
| Account Name filter       | Dropdown filter         | Filters history by a specific account                                   |
| LOAD MORE button          | Pagination              | Loads additional history records beyond initial view                    |
| Date column               | Table column            | Date the deposit was submitted                                          |
| Amount column             | Table column            | Dollar amount of the deposit                                            |
| Receipt No. column        | Table column            | Unique receipt identifier for the deposit transaction                   |
| Channel column            | Table column            | Deposit channel: Online Deposit / Mobile Deposit / Branch / ATM Deposit |
| Status column             | Table column            | Current deposit status: Submitted / Approved / Rejected                 |
| View Image column         | Action link             | Opens front and back check image thumbnails for the selected deposit    |

**5. QUICK REFERENCE**

|                        |                                                             |                     |                                                        |
| ---------------------- | ----------------------------------------------------------- | ------------------- | ------------------------------------------------------ |
| **Task**               | **Navigation Path**                                         | **Who Can Do It**   | **Notes**                                              |
| Submit a web deposit   | Check Deposit > Deposit Your Check tab > Fill & Submit    | RDC-enrolled member | Drag-drop or click to upload front/back images         |
| View deposit status    | Check Deposit > Check Deposit History tab                  | Member / Operations | Filter by date range and account name                  |
| View check images      | History tab > View Image column                            | Member / Compliance | Front and back thumbnails from deposit time            |
| Check deposit limit    | Deposit form — displayed automatically on account selection | Member              | Per account; set by Summerville FCU                    |
| Clear and restart form | Deposit form > Clear button                                | Member              | Resets all fields; does not cancel a submitted deposit |
