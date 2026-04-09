**SUMMERVILLE CREDIT UNION · BUSINESS BANKING USER GUIDE · CSUM-06 of
16**

**Role Management**

Module: Business Banking \> Role Management

**Navigation: Dashboard → Business Banking → Role Management**

*Sources: Summerville Reports Series A + Series B | Features: nFinia
Documentation Features Spreadsheet*

|                        |
| ---------------------- |
| **01 PRODUCT SUMMARY** |

Role Management is the administrative backbone of business banking
access control within the nFinia platform. It allows business
administrators to define roles (such as View-only, Basic Role, or custom
roles) that determine what features, transaction types, and monetary
limits each user can access. Each role encompasses four configurable
dimensions: Permissions (which features are accessible), Limits
(transaction amount thresholds per payment type), Users (which team
members are assigned to the role), and Settings (role-level
configuration).

The system ships with default roles (View-only with a lock icon
indicating it cannot be deleted) and supports unlimited custom role
creation. Business admins can granularly control access to ACH
transfers, wire transfers, bill pay, internal transfers, and
administrative functions. Transaction limits can be set per role for
daily, per-transaction, and cumulative thresholds.

For credit unions, role management is a critical differentiator that
enables them to serve multi-user businesses. It provides the
dual-control and segregation-of-duties capabilities that commercial
businesses require for regulatory compliance and internal fraud
prevention.

**At a Glance**

|                      |                                                                                                                                                          |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Attribute**        | **Detail**                                                                                                                                               |
| Feature Name         | Role Management                                                                                                                                          |
| Module               | Business Banking \> Role Management                                                                                                                      |
| Navigation           | Dashboard → Business Banking → Role Management                                                                                                           |
| User Roles           | Business Admin, Business Owner                                                                                                                           |
| Access Level         | Admin-only; requires Role Management permission                                                                                                          |
| Key Actions          | View roles, Create role, Edit role, Assign permissions, Set limits, Assign users, View user info, Edit user, Deactivate user, Remove user, Cancel invite |
| Regulatory Relevance | Dual-control compliance, segregation of duties, audit trail                                                                                              |

|                      |
| -------------------- |
| **02 KEY USE CASES** |

|                           |                 |                                                          |                                                         |
| ------------------------- | --------------- | -------------------------------------------------------- | ------------------------------------------------------- |
| **Use Case**              | **Who Uses It** | **What They Do**                                         | **Business Value**                                      |
| Create Custom Role        | Business Admin  | Add a new role with specific permissions and limits      | Tailors access to business organizational structure     |
| Set Transaction Limits    | Business Owner  | Configure per-role ACH, wire, and payment limits         | Enforces spending controls aligned with business policy |
| Assign Users to Role      | Business Admin  | Move team members into appropriate roles                 | Ensures each employee has correct level of access       |
| Audit Role Permissions    | Business Owner  | Review permissions and limits across all roles           | Supports compliance audits and internal controls review |
| View-only Access          | Business Admin  | Assign read-only role to bookkeepers or accountants      | Provides visibility without transaction authority       |
| View User Details         | Business Admin  | Review user profile, role assignment, and account access | Confirms correct user configuration                     |
| Edit User Role            | Business Admin  | Change a user's role or update contact information       | Adapts access as employee responsibilities change       |
| Deactivate User           | Business Admin  | Deactivate a user from one or more businesses            | Revokes access for departing employees immediately      |
| Remove User from Business | Business Admin  | Permanently disassociate a user from the business        | Ensures former employees have zero access               |
| Cancel Pending Invite     | Business Admin  | Cancel an outstanding invitation before acceptance       | Prevents unintended access from stale invitations       |

|                                |
| ------------------------------ |
| **03 STEP-BY-STEP USER GUIDE** |

**How to get here: Dashboard → Business Banking → Role Management**

**Step 1: Log In and Open the Dashboard**

Open your web browser and navigate to the Summerville Credit Union
digital banking platform. Enter your username and password on the login
screen and click "Log In." If prompted, complete the OTP (One-Time
Passcode) verification by entering the code sent to your registered
device. After successful authentication, you will land on the Dashboard
— also called the Account Overview screen. This is your home base. The
Dashboard displays all your business accounts (Savings Accounts,
Checking Accounts) with their available and current balances. The top
navigation bar shows links to Dashboard, Accounts, Transfer & Pay,
Cards, Business Banking, and More. On the right sidebar you will see
Related Links (Change Password, Account Settings, View Scheduled
Transfers, Account Specific Alerts) and a Quick Transfer widget for fast
internal transfers. To proceed to Business Banking features, locate the
"Business Banking" tab in the top navigation bar and click on it.

![Fig
1](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/1a19568ff18131f218abd77ce89a1be61f1d1d82.png
"Fig 1")

*Figure 1 — Log In and Open the Dashboard*

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

![Fig
2](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/4c26e21f2a941fd4d0531c900025b3d6ab137178.png
"Fig 2")

*Figure 2 — Open the Business Banking Hub*

**Step 3: Navigate to Role Management**

From the Dashboard, click "Business Banking" in the left-side navigation
menu to open the Business Banking Hub. In the "Manage" section, click
the "Role Management" tile. The Role Management dashboard appears,
listing all roles defined for your business. Each role is displayed as a
card showing the role name, the number of active users assigned to it,
and a lock icon for system-protected roles (like "View-only") that
cannot be deleted. You will see tabs on each card: Permissions, Limits,
Users, and Settings. Click any tab to expand that dimension for the
selected role. To create a new role, click "Create New Role" at the top
of the page.

![Fig
3](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/448d4b229fdaca1e425d06609b1b8907922c41d6.png
"Fig 3")

*Figure 3 — Navigate to Role Management*

**Step 4: View and Configure Role Permissions**

Click the "Permissions" tab on any role card to expand the permission
configuration panel. You will see a checklist of toggle switches for
every business banking feature: ACH Transfer (Send/Receive), Wire
Transfer, Transfer Templates, Payment From File, Role Management, User
Management, Approval Settings, Recipient Management, Commercial
Activity, Reports, Approvals, Business Alerts, and more. To enable a
feature for this role, toggle the switch to ON (active color). To remove
access, toggle it OFF (grayed out). A "Select All" option at the top
enables every permission at once. Changes are saved when you click
"Save" at the bottom of the panel.

![Fig
4](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/402ab9e6dba46fff8843e866afcd34df422a3b21.png
"Fig 4")

*Figure 4 — View and Configure Role Permissions*

**Step 5: Scroll to See All Permission Categories**

Scroll down within the Permissions panel to see additional permission
categories not visible in the initial view. These extended permissions
cover payment processing controls (can this role initiate vs. only
approve transactions), administrative access (can this role manage other
roles or users), reporting permissions (which report types are visible),
and alert configuration rights. Review every category to ensure the role
has exactly the access it needs — no more, no less. For example, an "AP
Clerk" role should have ACH Transfer and Recipient Management enabled,
but Role Management and User Management disabled.

![Fig
5](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/46f5b82e8142404dff26ef8410fbf64f8b6e7adf.png
"Fig 5")

*Figure 5 — Scroll to See All Permission Categories*

**Step 6: Set Transaction Limits for the Role**

Click the "Limits" tab on the role card. A table appears with rows for
each payment type (ACH Transfer, Wire Transfer, Internal Transfer, Bill
Pay) and columns for Per-Transaction Limit and Daily Cumulative Limit.
Click into each dollar amount field and type the appropriate limit
value. For example, set ACH Per-Transaction to $5,000 and ACH Daily
Cumulative to $25,000 for a basic role. These limits are enforced in
real-time — if a user assigned to this role attempts a transaction
exceeding these thresholds, the system will block it. Click "Save" when
finished. Adjust limits based on business need and risk tolerance.

![Fig
6](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/80dc6a42ea881bd076ce32e73ac573d68ab0c459.png
"Fig 6")

*Figure 6 — Set Transaction Limits for the Role*

**Step 7: View Users Assigned to the Role**

Click the "Users" tab on the role card to see all team members currently
assigned to this role. Each entry shows the user's name, email, and
status (Active, Locked, etc.). To add a user to this role, click "Add
User" and select from the list of unassigned users. To remove a user
from the role, click the remove button next to their name. Removing a
user from a role revokes all permissions associated with that role
immediately. The user will need to be reassigned to a different role to
regain access.

![Fig
7](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/92f042e8db546163b78620f48f6a6f3e999276d4.png
"Fig 7")

*Figure 7 — View Users Assigned to the Role*

**Step 8: Review Role Settings**

Click the "Settings" tab to view role-level configuration. Here you can
edit the role name and description. The description field should
document the role's purpose (e.g., "For accounts payable staff who
process vendor payments"). Settings may also include role-specific
behaviors like whether transactions initiated by this role require
approval from another role. Update the settings as needed and click
"Save."

![Fig
8](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/204f8f8c10e13f12f78d73928bad58dd90f1faa1.png
"Fig 8")

*Figure 8 — Review Role Settings*

**Step 9: Edit an Existing Role**

To modify an existing role, click the "Edit" button on the role card.
The role editor opens with all four dimensions (Permissions, Limits,
Users, Settings) in editable mode. Make your changes — add or remove
permissions, adjust limits, reassign users, or update the description.
When finished, click "Save" to apply changes. All changes take effect
immediately for all users assigned to this role. Be cautious when
editing roles with active users, as permission changes affect their
access in real-time.

![Fig
9](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/a9ff020e6922e6b539683dcc8ab0318a5e47bbd6.png
"Fig 9")

*Figure 9 — Edit an Existing Role*

**Step 10: Create a New Role — Enter the Role Name**

Click "Create New Role" from the Role Management dashboard. A creation
form opens. Enter a descriptive role name in the Name field (e.g., "AP
Clerk," "CFO," "Branch Manager," or "Auditor"). Choose a name that
clearly reflects the role's function within your organization, as this
name will appear throughout the platform wherever role assignments are
displayed. Click "Continue" or "Next" to proceed to permission
configuration.

![Fig
10](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/2ddca15f587d3f757e2862548ed30412d11b6f59.png
"Fig 10")

*Figure 10 — Create a New Role — Enter the Role Name*

**Step 11: Confirm the Role Name and Proceed**

The role name is now entered in the field. Verify the spelling and
clarity of the name. If it needs correction, click into the field and
edit it. When satisfied, click "Continue" to advance to the privilege
selection step. The role name can be changed later through the Settings
tab if needed, but it is best practice to set a clear, descriptive name
from the start to maintain an organized role structure.

![Fig
11](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/c173e7157610ddeec8de77fd5bc2d1877b035247.png
"Fig 11")

*Figure 11 — Confirm the Role Name and Proceed*

**Step 12: Select Feature Privileges for the New Role**

The privilege selection step presents high-level feature categories
organized into logical groups (Transfers, Management, Reporting, etc.).
Click the checkbox or toggle next to each feature group this role should
access. Within each selected group, individual features can be toggled
on or off for more granular control. A summary counter shows how many of
the total available privileges are enabled. Select only the features
necessary for this role's job function — following the principle of
least privilege minimizes security risk. Click "Continue" to proceed to
entitlement configuration.

![Fig
12](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/3454de4077a36ecdcfa37ff8658f3f3543fea0d7.png
"Fig 12")

*Figure 12 — Select Feature Privileges for the New Role*

**Step 13: Configure Detailed Entitlements and Save**

The entitlements step provides the finest level of access control.
Within each selected privilege group, individual actions are listed with
toggle switches. For example, within "ACH Transfer" you may see:
Initiate ACH Send, Initiate ACH Receive, Approve ACH, View ACH History,
and Cancel Pending ACH. Toggle each action on or off based on what this
role should be able to do. After configuring all entitlements, click
"Save" (or "Create Role") to finalize. The new role immediately appears
in the Role Management dashboard and is ready for users to be assigned
to it.

![Fig
13](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/4c4932f87df9f994c5ae85a9740838ea0c4211c0.png
"Fig 13")

*Figure 13 — Configure Detailed Entitlements and Save*

**Step 14: View User Information and Role Assignment**

From the User Management screen (Business Banking \> Manage Users),
click on any user to view their full profile. The User Information page
displays the user's initials badge, name, and quick-action links: "Edit
user" and "Deactivate user." Below, you see the Email ID, Mobile number,
and User ID. The "This user is associated with" section shows which
business membership the user belongs to (displayed as a clickable badge
with the business name and membership number). The "User role" section
shows the currently assigned role (e.g., "Basic Role") with a "View role
privileges" link to inspect what permissions that role grants. The
"Account access" section lists which specific accounts the user can see
— for example, Membership Share Savings Account (S0100) and Business
Money Market Account (S6500). This page is the central reference for
auditing any individual user's access configuration.

![Fig
14](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/486fe3e3ceffacfa404412718d5491fbc5d2cb4e.png
"Fig 14")

*Figure 14 — View User Information and Role Assignment*

**Step 15: Edit User Information and Role Assignment**

Click "Edit user" from the User Information page. The edit form opens
with editable fields for First Name, Last Name, Email address, Mobile
number, and User ID. Below the personal details, a "Select user role"
dropdown allows you to change the user's role assignment (e.g., switch
from "Basic Role" to a custom role like "AP Clerk" or "CFO"). A "View
role privileges" link lets you preview the permissions of the selected
role before saving. A yellow note at the bottom reminds administrators:
"Please ensure the user(s) is set up on other necessary systems, so they
may effectively access all digital banking features." After making
changes, click "Save" to apply. Role changes take effect immediately —
the user's permissions and limits update in real-time.

![Fig
15](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/fb83cc55634553a2e5bdd7fd66c469dfd66fd026.png
"Fig 15")

*Figure 15 — Edit User Information and Role Assignment*

**Step 16: Deactivate a User**

To deactivate a user, click "Deactivate user" from the User Information
page. A confirmation dialog appears showing the user's name and how many
businesses they are currently active with. The dialog lists each
business association with the user's role (e.g., "Dunder Mifflin, Inc.
(Basic Role)") and a selection checkbox. You can choose to deactivate
the user from specific businesses or all of them. Click the red
"Deactivate user" button to confirm, or "Cancel" to return. Deactivated
users lose all digital banking access immediately but remain in the
system for audit purposes. They can be reactivated later if needed. This
is the recommended action for temporary access removal, such as employee
leave.

![Fig
16](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/06a9ea7c68fbdd644d0930c9aef8fc95e23ee02d.png
"Fig 16")

*Figure 16 — Deactivate a User*

**Step 17: Remove User from Business**

For permanent disassociation, click the remove action on the user's
business badge. A warning dialog appears: "Remove user from business."
The message clearly states that this action will remove the user's
association with the business and that if performed, the user will not
be associated to any of your businesses and will no longer have digital
banking access to any of your business memberships. Click "Yes" to
confirm removal or "No" to cancel. Unlike deactivation, removal is a
more permanent action — the user must be re-invited and re-onboarded to
regain access. Use this for departed employees who will not return.

![Fig
17](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/8e81f1e6ad3e15e5d9216545977c804b05321009.png
"Fig 17")

*Figure 17 — Remove User from Business*

**Step 18: Manage Invited Users and Cancel Invitations**

Navigate to the User Management screen and click the "Invited users"
tab. This view displays all pending invitations organized by role: Basic
Role, custom roles (e.g., "testrole"), and View-only. Each invited user
card shows their name, assigned role, status (e.g., "Processing..."),
and two action links: "Resend invite" and "Cancel invite." To cancel a
pending invitation, click "Cancel invite." A confirmation dialog asks:
"Are you sure you want to cancel the invite for this user?" with "No"
and "Yes" buttons. Cancelling an invite prevents the user from
completing registration and gaining access. This is useful when an
invitation was sent in error or the intended user is no longer joining
the business. The Invited users tab also shows tabs for Active users,
New authorized signers, Locked users, and Deactivated users for complete
user lifecycle management.

![Fig
18](/sessions/eloquent-nifty-ptolemy/bb-conversions/CSUM-06-Business-Banking-Role-Management/media/94ee662f22837c28d52c035810e1836fecb89d9c.png
"Fig 18")

*Figure 18 — Manage Invited Users and Cancel Invitations*

**3.3 Decision Points & Branching**

• System-protected roles (View-only) cannot be deleted or renamed; only
custom roles are fully editable.

• Deactivating a user preserves their record for audit purposes;
removing a user permanently disassociates them from the business.

• Cancelling an invitation prevents the invited user from completing
registration; a new invitation must be sent if access is later needed.

• Role changes take effect immediately for all assigned users — test
changes on a single user before applying to a shared role.

**3.4 Completion & Confirmation**

When a role is created or edited, changes are saved and applied
instantly. When a user is deactivated, removed, or their invite is
cancelled, the system updates access controls in real-time. All changes
are logged in the audit trail for compliance review.

**3.5 Error Handling**

• Attempting to delete a system-protected role returns an error; only
custom roles can be removed.

• If a user being edited has active pending transactions, a warning
appears before role changes are applied.

• Network errors during save operations preserve the previous
configuration until a successful save completes.

|                                          |
| ---------------------------------------- |
| **04 FEATURE OVERVIEW (UI WALKTHROUGH)** |

**Role Management Dashboard**

The main screen listing all defined roles with expandable tabs for
Permissions, Limits, Users, and Settings.

|                     |                  |                                                                   |                            |
| ------------------- | ---------------- | ----------------------------------------------------------------- | -------------------------- |
| **Field / Element** | **Type**         | **Description**                                                   | **Notes**                  |
| Role Card           | Card             | Displays role name, user count, and lock icon for protected roles | Click tabs to expand       |
| Permissions Tab     | Expandable Panel | Toggle switches for each business banking feature                 | Select All available       |
| Limits Tab          | Expandable Panel | Per-transaction and daily cumulative limits by payment type       | Dollar amount fields       |
| Users Tab           | Expandable Panel | List of users assigned to this role with add/remove               | Immediate effect on access |
| Settings Tab        | Expandable Panel | Role name, description, and behavioral settings                   | Editable for custom roles  |
| Create New Role     | Button           | Opens the role creation wizard                                    | Top of page                |

**User Information Screen**

Detailed view of an individual user's profile, role, and account access.

|                             |              |                                              |                         |
| --------------------------- | ------------ | -------------------------------------------- | ----------------------- |
| **Field / Element**         | **Type**     | **Description**                              | **Notes**               |
| User Name & Initials        | Label        | Displays the user's name and initials badge  | Read-only               |
| Edit User                   | Link         | Opens the user edit form                     | Blue text link          |
| Deactivate User             | Link         | Opens deactivation confirmation dialog       | Preserves audit record  |
| Email ID / Mobile / User ID | Labels       | User's contact and login information         | Masked for security     |
| Business Association        | Badge        | Shows linked business with membership number | Clickable               |
| User Role                   | Label + Link | Current role with View role privileges link  | Shows active role       |
| Account Access              | List         | Specific accounts this user can see          | Account type shown      |
| Select User Role            | Dropdown     | Change role assignment (edit mode)           | Immediate effect        |
| Remove User from Business   | Dialog       | Permanently disassociates user               | Cannot be undone easily |
| Cancel Invite               | Link         | Cancels pending user invitation              | On Invited users tab    |

|                        |
| ---------------------- |
| **05 QUICK REFERENCE** |

|                           |                                    |                   |                       |
| ------------------------- | ---------------------------------- | ----------------- | --------------------- |
| **Task**                  | **Navigation Path**                | **Who Can Do It** | **Notes**             |
| View all roles            | BB Hub → Role Management           | Business Admin    | Shows role cards      |
| Create a new role         | Role Mgmt → Create New Role        | Business Admin    | 3-step wizard         |
| Edit role permissions     | Role card → Permissions tab        | Business Admin    | Toggle switches       |
| Set transaction limits    | Role card → Limits tab             | Business Admin    | Per-txn and daily     |
| View assigned users       | Role card → Users tab              | Business Admin    | Add/remove users      |
| View user details         | User Mgmt → Click user             | Business Admin    | Full profile view     |
| Edit user info & role     | User Info → Edit user              | Business Admin    | Change role dropdown  |
| Deactivate a user         | User Info → Deactivate user        | Business Admin    | Select businesses     |
| Remove user from business | User Info → Remove badge           | Business Admin    | Permanent removal     |
| Cancel pending invite     | User Mgmt → Invited users → Cancel | Business Admin    | Prevents registration |
