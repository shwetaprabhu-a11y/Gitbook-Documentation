# Phone Number Management Guide

### Summerville Credit Union — nFinia Personal Information

**Feature Area:** More > Personal Information > Contact Information\
**Platform:** nFinia by Tyfone\
**Prepared by:** Jeeva Krishnamurthy, Sr. Product Manager — Digital Banking\
**Date:** April 2026

***

## 1. Product Summary

The Phone Number Management feature within the nFinia platform enables Summerville Credit Union You to maintain accurate, up-to-date contact information directly through their online banking portal. You can add new phone numbers across four categories — Cellular, Home, Business, and Business Cell — edit existing numbers, and remove outdated ones, all without requiring a branch visit or call center interaction.

This feature serves retail You accessing the platform via the Personal Memberships profile. It is located under **More > Personal Information > Contact Information** and supports self-service contact data management, reducing operational load on credit union staff while improving data quality for fraud detection, OTP delivery, and member communications.

The business value for Summerville CU is significant: accurate phone numbers are foundational to two-factor authentication flows, real-time fraud alerts, and regulatory contact requirements. Every change — add, edit, or remove — is protected by an OTP verification step, creating an audit trail and protecting You from unauthorized modifications to their contact details.

| Attribute            | Detail                                                                       |
| -------------------- | ---------------------------------------------------------------------------- |
| Feature Name         | Phone Number Management (Add / Edit / Remove)                                |
| Module               | More > Personal Information > Contact Information                            |
| User Roles           | Retail Member (Personal Memberships)                                         |
| Access Level         | Authenticated member; OTP required for all changes                           |
| Key Actions          | Add new number, Edit existing number, Remove number                          |
| Phone Categories     | Cellular, Home, Business, Business Cell                                      |
| Regulatory Relevance | OTP/2FA delivery accuracy, BSA contact record integrity, fraud alert routing |

***

## 2. Use Cases

| Use Case                        | Who Uses It                                       | What They Do                                                                                                                        | Business Value                                                                                                      |
| ------------------------------- | ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Add a cellular number           | New member or member with no cellular on file     | Navigates to Contact Information, selects "Add a new phone number" under Cellular, enters country code and number, verifies via OTP | Ensures the credit union has a valid mobile number for fraud alerts and OTP delivery                                |
| Add a secondary business number | SMB member or member with business accounts       | Adds a number under the Business category to separate work and personal contact channels                                            | Supports segmented communication and accurate routing for business-related alerts                                   |
| Edit an existing phone number   | Member who changed their mobile carrier or number | Selects Edit next to the existing number, updates the number in the inline form, completes OTP verification                         | Keeps contact records current, reducing failed OTP deliveries and missed fraud alerts                               |
| Remove an outdated number       | Member who disconnected a phone line              | Selects Remove, confirms via modal dialog, completes OTP verification                                                               | Reduces clutter in contact records and eliminates risk of OTPs being sent to a number you no longer controls |
| OTP verification on change      | All You making any phone number change        | Selects delivery method (text or call), picks the target number, enters the 6-digit code                                            | Prevents unauthorized contact changes; creates an auditable security event                                          |
| Recover when OTP not received   | Member who does not receive the code              | Uses "Select another method" or waits for the retry countdown (58s) and requests a new code                                         | Reduces abandonment; keeps member in self-service channel                                                           |

Every phone number change in nFinia triggers an OTP challenge, ensuring that contact record updates are authenticated events — not silent modifications. This is particularly important for credit unions where phone numbers are the primary channel for fraud callbacks and secure message delivery.

***

## 3. End-to-End Workflow

### 3.1 Prerequisites

* Member must have an active Summerville CU online banking account
* Member must be able to complete OTP verification at login (pre-existing verified phone or email on file)
* To **edit or remove** a number, at least one phone number must already exist on the account
* To **add** a number, the target category (Cellular, Home, Business, Business Cell) must have an available "Add a new phone number" slot

***

### 3.2 Step-by-Step Flows

***

## Part A — Add a Phone Number

**Step 1 — Log In to Online Banking**

you navigates to the Summerville CU online banking portal and enters their User ID and password. They click **Log in**.

![Screenshot 1](<../../../.gitbook/assets/Screenshot_1_1 (1).png>)

***

**Step 2 — OTP Verification at Login (Method Selection)**

The system prompts for OTP verification before granting dashboard access. you selects how to receive the one-time passcode: **Send me a message**, **Call me**, or **Send me an email**.

![Screenshot 2](<../../../.gitbook/assets/Screenshot_2_2 (1).png>)

***

**Step 3 — OTP Phone Number Selection**

If you selects "Send me a message" or "Call me", they are presented with a list of masked phone numbers on file to choose the delivery destination.

![Screenshot 3](<../../../.gitbook/assets/Screenshot_3_3 (1).png>)

***

**Step 4 — Enter OTP Code**

A 6-digit OTP is sent to the selected number. you enters the code in the Enter code field and clicks **Submit**. A retry countdown (52 seconds) is shown if the code has not arrived. you can optionally check **Remember Device/Browser** to skip this step on future logins from the same device.

![Screenshot 4](<../../../.gitbook/assets/Screenshot_4_4 (1).png>)

***

**Step 5 — Dashboard Access**

After successful OTP entry, you lands on the Dashboard, showing their name, account balances, and navigation options.

![Screenshot 5](<../../../.gitbook/assets/Screenshot_5_5 (1).png>)

***

**Step 6 — Navigate via Profile Switcher (if applicable)**

If you have multiple profiles (Personal Memberships and/or Business accounts), they may see a profile selection panel. For phone number management, you selects **Personal Memberships**.

![Screenshot 6](<../../../.gitbook/assets/Screenshot_6_6 (1).png>)

***

**Step 7 — Navigate to Personal Information > Contact Information**

you clicks **More** in the top navigation, then selects **Personal Information**. The Contact Information tab is displayed by default, showing Primary phone, Primary email, and phone categories (Cellular, Home, Business, Business Cell). Categories without a number show an **Add a new phone number** radio button link.

![Screenshot 7](<../../../.gitbook/assets/Screenshot_7_7 (1).png>)

***

**Step 8 — Enter New Phone Number**

you clicks the **Add a new phone number** radio button under the desired category (e.g., Cellular). An inline form expands showing a **country code dropdown** (defaulting to United States +1) and a **phone number input field**. you enters the 10-digit number and clicks **Add new number**. A **Cancel** button is available to discard the entry.

![Screenshot 8](../../../.gitbook/assets/Screenshot_8_8.png)

***

**Step 9 — OTP Verification (Method Selection — Logged In)**

After submitting the new number, the system triggers an OTP challenge. you selects the delivery method: **Send me a message** or **Call me**. This OTP is distinct from the login OTP and specifically authorizes the contact change.

![Screenshot 9](../../../.gitbook/assets/Screenshot_9_9.png)

***

**Step 10 — OTP Phone Number Selection (Logged In)**

you selects which existing phone number should receive the OTP to authorize the change.

![Screenshot 10](../../../.gitbook/assets/Screenshot_10_10.png)

***

**Step 11 — Enter OTP Code to Authorize Change**

you enters the 6-digit code sent to the selected number. The retry countdown (58 seconds) is shown if needed.

![Screenshot 11](../../../.gitbook/assets/Screenshot_11_11.png)

***

**Step 12 — Confirmation**

The system returns to the Personal Information page and displays the success banner: **"New phone number has been added successfully."** The new number appears under its category with Edit and Remove links available.

![Screenshot 12](../../../.gitbook/assets/Screenshot_12_12.png)

***

## Part B — Edit a Phone Number

**Step 1 — Log In**

![Screenshot 1](../../../.gitbook/assets/Screenshot_1_13.png)

***

**Step 2 — OTP Verification at Login (Method Selection)**

![Screenshot 2](../../../.gitbook/assets/Screenshot_2_14.png)

***

**Step 3 — OTP Phone Number Selection**

![Screenshot 3](../../../.gitbook/assets/Screenshot_3_15.png)

***

**Step 4 — Enter OTP Code at Login**

![Screenshot 4](../../../.gitbook/assets/Screenshot_4_16.png)

***

**Step 5 — Dashboard**

![Screenshot 5](../../../.gitbook/assets/Screenshot_5_17.png)

***

**Step 6 — Profile Selection**

![Screenshot 6](../../../.gitbook/assets/Screenshot_6_18.png)

***

**Step 7 — Navigate to Personal Information > Contact Information**

The Contact Information tab shows existing phone numbers. Each number has **Edit** and **Remove** links. you clicks **Edit** next to the number they want to change.

![Screenshot 7](<../../../.gitbook/assets/Screenshot_7_19 (1).png>)

***

**Step 8 — Update Phone Number Inline**

The phone number row expands into an editable inline form pre-populated with the existing number. The country code dropdown (United States +1) remains selectable. you clears the current number and enters the updated one, then clicks **Update** (or **Cancel** to abort).

![Screenshot 8](<../../../.gitbook/assets/Screenshot_8_20 (1).png>)

***

**Step 9 — OTP Verification (Method Selection)**

Submitting the update triggers an OTP challenge to authorize the change. you selects delivery method.

![Screenshot 9](../../../.gitbook/assets/Screenshot_9_21.png)

***

**Step 10 — OTP Phone Number Selection**

![Screenshot 10](../../../.gitbook/assets/Screenshot_10_22.png)

***

**Step 11 — Enter OTP Code**

![Screenshot 11](../../../.gitbook/assets/Screenshot_11_23.png)

***

**Step 12 — Confirmation**

The system returns to Personal Information and displays: **"Phone number has been updated successfully."** The updated number is shown in the relevant category row.

![Screenshot 12](../../../.gitbook/assets/Screenshot_12_24.png)

***

## Part C — Remove a Phone Number

**Step 1 — Log In**

![Screenshot 1](../../../.gitbook/assets/Screenshot_1_25.png)

***

**Step 2 — OTP Verification at Login (Method Selection)**

![Screenshot 2](../../../.gitbook/assets/Screenshot_2_26.png)

***

**Step 3 — OTP Phone Number Selection**

![Screenshot 3](../../../.gitbook/assets/Screenshot_3_27.png)

***

**Step 4 — Enter OTP Code at Login**

![Screenshot 4](../../../.gitbook/assets/Screenshot_4_28.png)

***

**Step 5 — Dashboard**

![Screenshot 5](../../../.gitbook/assets/Screenshot_5_29.png)

***

**Step 6 — Profile Selection**

![Screenshot 6](../../../.gitbook/assets/Screenshot_6_30.png)

***

**Step 7 — Navigate to Personal Information > Contact Information**

The Contact Information tab lists all existing numbers. you clicks **Remove** next to the number they want to delete.

![Screenshot 7](<../../../.gitbook/assets/Screenshot_7_31 (1).png>)

***

**Step 8 — Confirmation Modal**

A modal dialog appears: **"Do you want to remove this phone number?"** with **Cancel** and **Confirm** buttons. This prevents accidental deletion.

![Screenshot 8](<../../../.gitbook/assets/Screenshot_8_32 (1).png>)

***

**Step 9 — OTP Verification (Method Selection)**

After confirming the modal, the system triggers an OTP challenge. you selects the delivery method.

![Screenshot 9](../../../.gitbook/assets/Screenshot_9_33.png)

***

**Step 10 — OTP Phone Number Selection**

![Screenshot 10](../../../.gitbook/assets/Screenshot_10_34.png)

***

**Step 11 — Enter OTP Code**

![Screenshot 11](../../../.gitbook/assets/Screenshot_11_35.png)

***

**Step 12 — Confirmation**

The system returns to Personal Information and displays: **"Phone number has been removed successfully."** The number is no longer shown in its category; an **Add a new phone number** link reappears in its place.

![Screenshot 12](../../../.gitbook/assets/Screenshot_12_36.png)

***

### 3.3 Decision Points & Branching

* **OTP delivery method:** If you have only phone numbers on file (no email), the login OTP screen will show only "Send me a message" and "Call me" — no email option. If you have email registered, "Send me an email" appears as a third option.
* **Add vs. Edit availability:** The "Add a new phone number" link only appears if the category has no number. Once a number exists, only Edit and Remove are shown.
* **Cancel at any point:** you can click Cancel during the inline form entry to discard changes without triggering an OTP challenge.
* **OTP retry:** If the code is not received within the countdown window, a "Retry" option becomes active. you can also select another delivery method.

### 3.4 Completion & Confirmation

Each successful operation results in a green-background inline banner at the top of the Personal Information page:

* Add: _"New phone number has been added successfully."_
* Edit: _"Phone number has been updated successfully."_
* Remove: _"Phone number has been removed successfully."_

The change is reflected immediately in the Contact Information display. No page reload is required.

### 3.5 Error Handling

| Scenario                     | What you Sees                                   | Recovery                                                                  |
| ---------------------------- | ------------------------------------------------------ | ------------------------------------------------------------------------- |
| OTP code entered incorrectly | Error message on the OTP entry screen                  | Re-enter the correct code or request a new one after the countdown        |
| OTP not received in time     | Countdown timer with "Retry" option                    | Wait for the timer to expire, then click Retry; or switch delivery method |
| Invalid phone number format  | Inline field validation error                          | Correct the number format and resubmit                                    |
| Cancel during flow           | Returns to Contact Information with no changes applied | you can restart the add/edit/remove action                             |

***

## 4. Feature Overview — UI Walkthrough

### Login Screen

The entry point for all phone management workflows. You authenticate with User ID and password before any contact information can be viewed or modified.

| Field / Element        | Type           | Description                        | Notes                                               |
| ---------------------- | -------------- | ---------------------------------- | --------------------------------------------------- |
| User ID field          | Text input     | your online banking username   | Pre-filled if "Save User ID" was previously enabled |
| Password field         | Password input | your account password          | Masked; show/hide toggle available                  |
| Log in button          | Button         | Submits credentials                | Disabled until both fields are populated            |
| I need help logging in | Link           | Navigates to account recovery flow | Available pre-authentication                        |
| Enroll button          | Button         | Initiates new member enrollment    | Top-right corner                                    |

***

### OTP Verification — Method Selection Screen (Pre-Login)

Displayed immediately after credential submission. Protects dashboard access with a second factor.

| Field / Element   | Type          | Description                             | Notes                                   |
| ----------------- | ------------- | --------------------------------------- | --------------------------------------- |
| Send me a message | Option button | Sends OTP via SMS to a registered phone | Shown if phone number exists on account |
| Call me           | Option button | Delivers OTP via automated voice call   | Shown if phone number exists on account |
| Send me an email  | Option button | Sends OTP to registered email address   | Shown if email exists on account        |

***

### OTP Verification — Phone Number Selection Screen

Shown when you selects "Send me a message" or "Call me". Lists masked phone numbers available for OTP delivery.

| Field / Element                             | Type               | Description                                         | Notes                                                |
| ------------------------------------------- | ------------------ | --------------------------------------------------- | ---------------------------------------------------- |
| Phone number options                        | Selectable list    | Masked phone numbers (e.g., (+1) 4\*\*-\*\*\*-\*61) | Displayed as partial numbers to protect privacy      |
| Select another method                       | Link               | Returns to method selection                         | Allows member to switch to email or another phone    |
| Don't see your updated contact information? | Informational link | Triggers a refresh from the core system             | Useful when numbers were recently updated via branch |

***

### OTP Code Entry Screen

Displayed after the delivery method and target number are selected.

| Field / Element                       | Type             | Description                                           | Notes                                           |
| ------------------------------------- | ---------------- | ----------------------------------------------------- | ----------------------------------------------- |
| Enter code                            | 6-box input      | One character per digit of the OTP                    | Auto-advances between boxes on input            |
| Didn't receive your code? Retry in Xs | Countdown + link | Allows requesting a new OTP after countdown expires   | Timer resets on each new code request           |
| Remember Device/Browser               | Checkbox         | Skips OTP challenge on future logins from this device | Only shown at login OTP, not during change OTPs |
| Submit                                | Button           | Submits the OTP for verification                      | Disabled until all 6 digits are entered         |

***

### Personal Information — Contact Information Tab

The primary screen for viewing and managing phone numbers. Accessed via **More > Personal Information**.

| Field / Element                                        | Type                 | Description                                                      | Notes                                                             |
| ------------------------------------------------------ | -------------------- | ---------------------------------------------------------------- | ----------------------------------------------------------------- |
| Contact information tab                                | Tab                  | Default active tab showing phone and email fields                | Other tabs: Address, Residential address, Devices, Trusted Device |
| Primary phone                                          | Dropdown/Label       | Displays you's primary phone (masked)                     | Can be changed via dropdown if multiple numbers exist             |
| Primary email                                          | Dropdown/Label       | Displays you's primary email (masked)                     | Read-only in this context                                         |
| Cellular / Home / Business / Business Cell             | Category labels      | Sections grouping phone numbers by type                          | Each category can hold one number                                 |
| Add a new phone number                                 | Radio-style link     | Expands inline form to add a number to that category             | Only shown when the category has no number                        |
| [Number] Edit \| Remove                               | Inline links         | Edit or remove the displayed number                              | Shown when a number exists in that category                       |
| Don't see your updated contact information? Click here | Informational banner | Triggers a fetch from the core banking system                    | Useful after branch or CSR-initiated changes                      |
| Related links (sidebar)                                | Link panel           | Change Password, Download E-Statements, View Scheduled Transfers | Persistent right-side panel                                       |

***

### Add / Edit Inline Form

Expands within the Contact Information tab when "Add a new phone number" or "Edit" is clicked.

| Field / Element         | Type       | Description                                               | Notes                                     |
| ----------------------- | ---------- | --------------------------------------------------------- | ----------------------------------------- |
| Country code dropdown   | Dropdown   | Country dial code selector (defaults to United States +1) | Supports international numbers            |
| Phone number input      | Text input | 10-digit number field                                     | Numeric only; validated before submission |
| Add new number / Update | Button     | Submits the new or updated number                         | Triggers OTP challenge on submission      |
| Cancel                  | Button     | Dismisses the inline form without saving                  | No OTP triggered                          |

***

### Remove Confirmation Modal

Appears when you clicks Remove on an existing phone number.

| Field / Element | Type   | Description                                   | Notes                                    |
| --------------- | ------ | --------------------------------------------- | ---------------------------------------- |
| Modal heading   | Text   | "Do you want to remove this phone number?"    | Prevents accidental deletion             |
| Cancel          | Button | Closes modal without removing the number      | Safe exit                                |
| Confirm         | Button | Proceeds with removal; triggers OTP challenge | Styled as primary action (filled button) |

***

## 5. Quick Reference

| Task                           | Navigation Path                                                                          | Who Can Do It               | Notes                                      |
| ------------------------------ | ---------------------------------------------------------------------------------------- | --------------------------- | ------------------------------------------ |
| Add a new phone number         | More > Personal Information > Contact Information > [Category] > Add a new phone number | Authenticated retail member | OTP required; country code selectable      |
| Edit an existing phone number  | More > Personal Information > Contact Information > [Number] > Edit                     | Authenticated retail member | OTP required; inline form pre-populated    |
| Remove a phone number          | More > Personal Information > Contact Information > [Number] > Remove                   | Authenticated retail member | Confirmation modal + OTP required          |
| Switch OTP delivery method     | Verification screen > Select another method                                              | Any member during OTP flow  | Returns to method selection screen         |
| Refresh contact info from core | Contact Information > Click here (banner)                                                | Any authenticated member    | Pulls latest data from core banking system |

***

_This guide was prepared using the nFinia platform as deployed at Summerville Credit Union. Screen behavior and field availability may vary based on individual member profile configuration and account type._
