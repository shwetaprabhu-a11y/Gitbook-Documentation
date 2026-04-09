**SUMMERVILLE CREDIT UNION · BUSINESS BANKING USER GUIDE · CSUM-08 of
16**

**Approval Settings**

Module: Business Banking \> Approvals \> Approval Settings

**Navigation: Dashboard → Business Banking → Approval Settings**

*Sources: Summerville Reports Series A + Series B | Features: nFinia
Documentation Features Spreadsheet*

|                        |
| ---------------------- |
| **01 PRODUCT SUMMARY** |

Approval Settings enables business administrators to configure
dual-control requirements for different transaction types. The feature
allows the business to specify how many approvals are required before a
transaction is processed, supporting values from 1 (auto-approved) to
multiple approvers for high-risk transaction types.

The settings screen displays each transaction type (ACH Payment, ACH
Collection, ACH Payroll, Domestic Wires) with a dropdown to set the
required number of approvals. When set to 1, transactions initiated by
an approver are auto-approved. Higher values enforce multi-party
authorization before any payment is released.

For credit unions, approval settings provide the dual-control framework
that regulators expect for commercial banking operations. This feature
directly addresses NCUA examination requirements for business account
controls and helps credit unions demonstrate adequate safeguards for
commercial payment processing.

**At a Glance**

|                      |                                                                |
| -------------------- | -------------------------------------------------------------- |
| **Attribute**        | **Detail**                                                     |
| Feature Name         | Approval Settings                                              |
| Module               | Business Banking \> Approvals \> Approval Settings             |
| Navigation           | Dashboard → Business Banking → Approval Settings               |
| User Roles           | Business Admin, Business Owner                                 |
| Key Actions          | Configure approval thresholds, Save, Reset                     |
| Regulatory Relevance | Dual-control enforcement, NCUA audit trail, BSA/AML safeguards |

|                  |
| ---------------- |
| **02 USE CASES** |

|                      |                 |                                                                      |                                         |
| -------------------- | --------------- | -------------------------------------------------------------------- | --------------------------------------- |
| **Use Case**         | **Who Uses It** | **What They Do**                                                     | **Business Value**                      |
| Initial Setup        | Business Admin  | Sets approval thresholds for each transaction type during onboarding | Establishes dual-control from day one   |
| Policy Update        | Business Owner  | Adjusts thresholds as business risk profile changes                  | Adapts controls to evolving needs       |
| High-Risk Protection | Business Admin  | Sets Domestic Wires to require 2+ approvals                          | Prevents unauthorized wire transfers    |
| Streamline Low-Risk  | Business Owner  | Sets ACH Payment to 1 for auto-approval of routine vendor payments   | Reduces friction for trusted operations |
| Audit Compliance     | FI Operations   | Reviews approval configuration for examination                       | Demonstrates regulatory compliance      |

These use cases reflect the approval settings configuration lifecycle —
from initial setup to ongoing policy adjustments. For approval request
queue management (reviewing, approving, and declining transactions), see
CSUM-10 Business Banking Approvals.

|                            |
| -------------------------- |
| **03 END-TO-END WORKFLOW** |

**3.1 Prerequisites**

• Active Summerville FCU business banking membership

• Business Admin or Business Owner role assigned

• At least one approver with approval permissions configured in Role
Management

**3.2 Step-by-Step Flow**

**Step 1: Log In to Summerville FCU Dashboard**

Navigate to the Summerville Federal Credit Union digital banking portal
and log in with your credentials. Once authenticated, the system loads
the personalized Dashboard showing account balances, quick transfer,
upcoming payments, and credit score. The Dashboard is the central hub
for all banking operations — every workflow begins here.

![fig1\_dashboard.png](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-08-Business-Banking-Approval-Settings/media/1a19568ff18131f218abd77ce89a1be61f1d1d82.png
"fig1_dashboard.png")

*Figure 1 — Summerville FCU Dashboard*

**Step 2: Open the Business Banking Hub**

After clicking "Business Banking" in the top navigation bar, the
Business Banking Hub loads. This is the central command center for all
commercial banking operations. The Hub is organized into three sections:
"Transfers" at the top (with tiles for ACH Transfer, Domestic Wire
Transfer, Transfer Template, and Payment From File), "Manage" in the
middle (with tiles for Role Management, User Management, Approval
Settings, and Recipient Management), and "More Options" at the bottom
(with tiles for Commercial Activity, Reports, and Approvals). Each tile
is a direct entry point to its corresponding feature. Only tiles your
role has permission to access will be visible. From here, locate and
click the tile for the feature you need — the next steps will guide you
through the specific workflow.

![fig2\_bb\_hub.png](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-08-Business-Banking-Approval-Settings/media/4c26e21f2a941fd4d0531c900025b3d6ab137178.png
"fig2_bb_hub.png")

*Figure 2 — Business Banking Hub*

**Step 3: Navigate to Approval Settings**

From the Dashboard, click "Business Banking" in the left-side navigation
menu to open the Business Banking Hub. In the "Manage" section, click
the "Approval Settings" tile. The Approval Settings page appears with a
table-style layout. Each row represents a transaction type: ACH Payment,
ACH Collection, ACH Payroll, and Domestic Wires. Next to each type is a
dropdown selector. Click the dropdown for any transaction type to set
the required number of approvals. Setting "1" means transactions
initiated by an authorized approver are auto-approved — no second person
is needed. Setting "2" means every transaction of that type requires a
second authorized user to approve it through the Approvals queue before
it is processed.

![fig3\_approval\_settings.png](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-08-Business-Banking-Approval-Settings/media/e8a9398b3d8ef1e97ccfe43db5eaadc2a978be71.png
"fig3_approval_settings.png")

*Figure 3 — Approval Settings Page*

**Step 4: Configure Thresholds and Save**

Review the complete Approval Settings page. Use the dropdown next to
each transaction type to set the appropriate threshold based on your
business risk policy. Recommended practice: set Domestic Wires to "2"
(dual-control for irrevocable high-value payments), and consider setting
ACH Payment to "1" for routine low-risk vendor payments. Read the
explanatory note at the top of the page — it describes how auto-approval
works when the threshold is set to 1. After adjusting all thresholds,
click "Save" to apply your changes. Click "Reset" if you want to revert
to the previous configuration. These settings take effect immediately
for all future transactions.

![fig4\_thresholds.png](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-08-Business-Banking-Approval-Settings/media/ddd8ab4a06611644970b2d15112e5d20cf5c17a9.png
"fig4_thresholds.png")

*Figure 4 — Configure Thresholds and Save*

**3.3 Decision Points & Branching**

• If the threshold is set to 1 and the initiator is an authorized
approver, the transaction is auto-approved with no queue entry.

• If the threshold is 2 or higher, the transaction enters the Pending
queue and requires the specified number of additional approvals before
processing.

• For managing approval requests (reviewing, approving, declining
pending transactions), refer to CSUM-10 Business Banking Approvals.

**3.4 Completion & Confirmation**

When approval thresholds are saved, changes take effect immediately for
all future transactions. A confirmation message appears on screen.
Existing pending requests are not retroactively affected — they continue
to require the number of approvals that were in effect when the
transaction was initiated.

**3.5 Error Handling**

• If a user without approval permissions attempts to access Approval
Settings, the tile is not visible in the Business Banking Hub.

• If the system cannot save threshold changes (e.g., network issue), an
error message appears and the previous settings remain in effect.

|                                          |
| ---------------------------------------- |
| **04 FEATURE OVERVIEW (UI WALKTHROUGH)** |

**Approval Settings Screen**

The main configuration screen where administrators set the required
number of approvals per transaction type.

|                     |          |                                                     |                                        |
| ------------------- | -------- | --------------------------------------------------- | -------------------------------------- |
| **Field / Element** | **Type** | **Description**                                     | **Notes**                              |
| Business Name       | Label    | Displays the business membership name and number    | Read-only                              |
| ACH – Payment       | Dropdown | Number of approvals for ACH payment transactions    | 1 = auto-approved                      |
| ACH – Collection    | Dropdown | Number of approvals for ACH collection transactions | 1 = auto-approved                      |
| ACH – Payroll       | Dropdown | Number of approvals for ACH payroll transactions    | 1 = auto-approved                      |
| Domestic Wires      | Dropdown | Number of approvals for domestic wire transfers     | Recommended: 2+                        |
| Save Button         | Button   | Applies the current threshold configuration         | Takes effect immediately               |
| Reset Button        | Button   | Reverts to previously saved settings                | Does not affect processed transactions |

|                        |
| ---------------------- |
| **05 QUICK REFERENCE** |

|                                 |                                                  |                                |                              |
| ------------------------------- | ------------------------------------------------ | ------------------------------ | ---------------------------- |
| **Task**                        | **Navigation Path**                              | **Who Can Do It**              | **Notes**                    |
| Configure approval thresholds   | Dashboard → Business Banking → Approval Settings | Business Admin, Business Owner | Changes apply immediately    |
| Reset settings                  | Approval Settings → Reset                        | Business Admin                 | Reverts to last saved config |
| Review/approve/decline requests | Dashboard → Business Banking → Approvals         | Authorized Approver            | See CSUM-10 Approvals        |
