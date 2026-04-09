**Summerville Federal Credit Union**

Push Notifications — Feature Report

nFinia Digital Banking Platform | April 2026

**1. Product Summary**

Push Notifications is a real-time communication feature within the
nFinia Digital Banking Platform that enables Summerville Federal Credit
Union to send targeted alerts and messages directly to You mobile
devices. The feature leverages Prisma, Tyfone integrated marketing and
communication engine, to configure, test, and deliver push notifications
through the Tyfone delivery channel.

This capability serves both FI Operations staff (who configure and test
push delivery through the Prisma Admin Portal) and end-user You (who
receive timely alerts on their iOS and Android mobile banking
applications). Push notifications are critical for member engagement,
fraud alerting, transaction confirmations, promotional campaigns, and
real-time account activity updates.

For Summerville FCU, push notifications represent a significant channel
for proactive member communication — reducing reliance on SMS and email
while providing a richer, more secure notification experience directly
within the branded mobile banking app. The feature is currently
validated in the UAT environment (Jira: SUP-37427) with production
rollout pending credit union confirmation.

**At a Glance**

|                      |                                                                 |
| -------------------- | --------------------------------------------------------------- |
| **Attribute**        | **Detail**                                                      |
| Feature Name         | Push Notifications                                              |
| Module               | Prisma Admin Portal > Settings > Push Notifications Setup     |
| Jira Reference       | SUP-37427 — Prisma Push Notification Setup                      |
| Status               | Development Complete — UAT Validated                            |
| User Roles           | FI Operations (Prisma Admin), Mobile Banking You            |
| Delivery Channel     | Tyfone (via Prisma integration)                                 |
| Platform             | iOS and Android Mobile Banking (nFinia)                         |
| Regulatory Relevance | Reg E alerts, fraud notification compliance, GLBA data security |

**2. Use Cases**

|                               |                                |                                                                                                                                       |                                                                                                  |
| ----------------------------- | ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| **Use Case**                  | **Who Uses It**                | **What They Do**                                                                                                                      | **Business Value**                                                                               |
| Transaction Alert Delivery    | Mobile Banking Member          | Receives real-time push notification for deposits, withdrawals, and transfers on their enrolled device                                | Immediate transaction awareness; reduces fraud exposure and support call volume                  |
| Prisma Push Configuration     | FI Operations / Admin          | Configures the Tyfone delivery channel in Prisma with Base URL, Client ID, and credentials; enables tokenized customer identification | One-time setup enables all push notification campaigns across you base                    |
| Test Push Notification        | FI Operations / QA             | Sends a test push notification to a specific member Individual ID from the Prisma Admin Portal to validate end-to-end delivery        | Verifies push pipeline before production rollout; prevents failed notifications reaching You |
| Marketing Campaign Push       | FI Marketing / Operations      | Creates and sends promotional push notifications (loan offers, rate changes, product announcements) to targeted member segments       | Higher engagement rates than email/SMS; drives product adoption and cross-sell                   |
| Fraud Alert Notification      | Mobile Banking Member          | Receives immediate push alert for suspicious activity, login attempts, or blocked transactions                                        | Enables rapid member response to fraud; meets Reg E notification requirements                    |
| Production Rollout Validation | FI Operations / Tyfone Support | Credit Union tests push delivery in UAT, confirms functionality, and authorizes production deployment                                 | Controlled rollout reduces risk; CU maintains oversight of go-live timing                        |

These use cases reflect the full lifecycle of push notification
management — from initial Prisma configuration by FI Operations, through
UAT validation, to production delivery of transactional and marketing
alerts to Summerville FCU You.

**3. End-to-End Workflow**

**3.1 Prerequisites**

|                         |                                                                                                               |
| ----------------------- | ------------------------------------------------------------------------------------------------------------- |
| **Prerequisite**        | **Detail**                                                                                                    |
| Prisma Admin Access     | FI Operations user must have admin credentials for the Prisma portal                                          |
| Tyfone Delivery Channel | Tyfone must be available as a delivery channel option in Prisma settings                                      |
| Base URL Configuration  | The credit union UAT or Production base URL must be provisioned (e.g., https://summervillefcutest.tyfone.com) |
| Client ID & Credentials | Client ID (e.g., SUMMERVILLEFCU) and password must be provided by Tyfone                                      |
| Mobile App Installation | Test users must have the Summerville FCU mobile banking app installed with push notifications enabled         |
| Member Individual ID    | The unique Individual ID of the test member must be known for test push delivery                              |

**3.2 Step-by-Step Flow**

|          |                              |                                                                                     |                                                                                           |
| -------- | ---------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| **Step** | **Screen / View**            | **Action**                                                                          | **System Response**                                                                       |
| 1        | Prisma Admin Portal — Login  | FI Operations user logs into the Prisma Admin Portal                                | Prisma authenticates and displays the admin dashboard                                     |
| 2        | Settings Menu                | Navigate to Settings in the left sidebar                                            | Settings submenu expands showing configuration options                                    |
| 3        | Push Notifications Setup     | Click "Push Notifications Setup" in the settings list                               | Displays the "Define Push Notifications Configuration" form                               |
| 4        | Configuration Form           | Select "Tyfone" from the Delivery Channel dropdown                                  | Form reveals Base URL, Client ID, Password fields, and Tokenize checkbox                  |
| 5        | Configuration Form           | Enter Base URL, Client ID, Password; check "Tokenize customer identifier"           | Fields are populated; tokenization ensures secure member ID handling                      |
| 6        | Configuration Form           | Click "Test Push Notification" button                                               | Modal dialog opens: "Test Push Notification Delivery"                                     |
| 7        | Test Push Notification Modal | Enter you Unique Identifier (Individual ID) and review pre-populated message | Message field shows: "Prisma: Summerville Push Notification Test {system.current-date}"   |
| 8        | Test Push Notification Modal | Click "Send Test"                                                                   | System dispatches push notification through Tyfone channel to the specified member device |
| 9        | Member Mobile Device         | Member receives push notification on lock screen / notification centre              | Notification displays with Summerville FCU app icon, app name, and message content        |

**3.3 Decision Points & Branching**

If the Tyfone delivery channel is not available in the dropdown, the
credit union must contact Tyfone support to enable it. If the test push
notification fails to deliver, verify: (a) the Base URL is correct for
the target environment (UAT vs. Production), (b) the Client ID and
password are valid, (c) you have the mobile app installed with
push notifications enabled, and (d) the Individual ID is correct.
Multiple test notifications can be sent to validate different member
accounts.

**3.4 Completion & Confirmation**

Upon successful test delivery, you device displays the push
notification with the Summerville FCU app icon and message content. The
FI Operations team confirms receipt with the test member and documents
validation results. Once UAT testing is confirmed, Tyfone coordinates
the production rollout — pointing the configuration to the production
Base URL and deploying to the live member base.

**3.5 Error Handling**

|                            |                                                     |                                                                                                               |
| -------------------------- | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| **Error Scenario**         | **User Experience**                                 | **Resolution**                                                                                                |
| Invalid Credentials        | Push test fails silently or returns error in Prisma | Verify Client ID and Password with Tyfone support; regenerate credentials if needed                           |
| Wrong Base URL             | Notification sent but not received on device        | Confirm correct environment URL (UAT vs. Prod) with Tyfone deployment team                                    |
| Push Not Enabled on Device | No notification appears on your phone             | Member must enable push notifications for the Summerville FCU app in device Settings                          |
| Invalid Individual ID      | Test push dispatched but no recipient matched       | Verify you Individual ID in the core banking system; ensure you have an active mobile enrollment |
| App Not Installed          | Push token not registered; delivery fails           | Member must download and install the Summerville FCU mobile app from App Store / Google Play                  |

**4. Feature Overview — UI Walkthrough**

**4.1 Prisma Push Notifications Setup Screen**

This screen is the primary configuration interface within the Prisma
Admin Portal. It allows FI Operations to define the push notification
delivery channel, authenticate with Tyfone, and initiate test
notifications.

![](/.gitbook/assets/e5ae27c7b7f0533f28471dd480ceb5426df96899.png)

*Figure 1: Prisma Admin Portal — Push Notifications Setup Configuration*

|                              |                |                                                                   |                                                             |
| ---------------------------- | -------------- | ----------------------------------------------------------------- | ----------------------------------------------------------- |
| **Field / Element**          | **Type**       | **Description**                                                   | **Notes**                                                   |
| Delivery Channel             | Dropdown       | Selects the push notification provider                            | Must select "Tyfone" for nFinia platform integration        |
| Base URL                     | Text Input     | The credit union Tyfone environment endpoint                      | UAT and Production URLs differ; confirm with Tyfone         |
| Client ID                    | Text Input     | Unique identifier for the credit union in Tyfone system           | Assigned by Tyfone during onboarding (e.g., SUMMERVILLEFCU) |
| Password                     | Password Input | Authentication credential for the Tyfone API                      | Stored securely; must be rotated per security policy        |
| Tokenize customer identifier | Checkbox       | Enables tokenized handling of member IDs for secure push delivery | Recommended: always enabled for PII protection              |
| Test Push Notification       | Button         | Opens the test notification delivery modal                        | Used during UAT validation and production smoke testing     |

**4.2 Test Push Notification Delivery Modal**

This modal dialog appears when the "Test Push Notification" button is
clicked. It allows FI Operations to send a test push to a specific
member device by entering their Individual ID.

![](/.gitbook/assets/a2e8c62678ac84a8bfb659e4b95f6d4eb6c9fc12.png)

*Figure 2: Test Push Notification Delivery Modal*

|                     |              |                                                       |                                                                            |
| ------------------- | ------------ | ----------------------------------------------------- | -------------------------------------------------------------------------- |
| **Field / Element** | **Type**     | **Description**                                       | **Notes**                                                                  |
| Unique Identifier   | Text Input   | you Individual ID to receive the test push     | Must match an active member with mobile app enrolled                       |
| Message             | Text Display | Pre-populated test message with dynamic date stamp    | Format: "Prisma: Summerville Push Notification Test {system.current-date}" |
| Send Test           | Button       | Dispatches the test notification to you device | Triggers real-time delivery through Tyfone channel                         |
| Close               | Button       | Closes the modal without sending                      | No notification is dispatched                                              |

**4.3 Mobile Push Notification — Notification Centre View**

When push notifications are delivered to you device, they appear
grouped in the iOS Notification Centre under the Summerville CU section.
Each notification card displays the Summerville FCU branded app icon,
the credit union name "Summerville CU", the notification message
content, and a delivery timestamp. The screenshot below shows successful
delivery of multiple Summerville CU push notifications grouped on a
member iOS device.

![](/.gitbook/assets/06544a40cc00e9658819cf4aa56f23e1e8844e7b.png)

*Figure 3: Summerville CU Push Notifications Grouped in iOS Notification
Centre*

|                      |                                                                                              |                                                                                 |
| -------------------- | -------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| **UI Element**       | **Description**                                                                              | **Notes**                                                                       |
| App Icon             | Summerville FCU branded icon displayed alongside each notification                           | Uses the mobile app icon configured during app build                            |
| App Name             | "Summerville CU" displayed as the notification source                                        | Matches the Summerville FCU mobile banking app display name                     |
| Notification Message | Real-world alert content including Withdrawal, Security, Payment Due, and Low Balance alerts | Production messages contain actual alert content tailored to member activity    |
| Timestamp            | Relative delivery time shown on each notification card (e.g. 3h ago, 5:12 PM)                | iOS groups Summerville CU notifications with "Show less" collapse option        |
| Notification Centre  | Notifications are accessible from the lock screen or by swiping down from any screen         | you can tap any notification to open the Summerville FCU mobile app directly |

**5. Quick Reference**

|                              |                                                    |                        |                                                       |
| ---------------------------- | -------------------------------------------------- | ---------------------- | ----------------------------------------------------- |
| **Task**                     | **Navigation Path**                                | **Who Can Do It**      | **Notes**                                             |
| Configure Push Channel       | Prisma > Settings > Push Notifications Setup     | FI Operations Admin    | One-time setup; select Tyfone delivery channel        |
| Send Test Push               | Push Notifications Setup > Test Push Notification | FI Operations / QA     | Enter member Individual ID; verify delivery on device |
| Receive Push Notification    | Summerville FCU Mobile App (iOS/Android)           | Mobile Banking Member  | Push must be enabled in device settings               |
| View Notification History    | Device Notification Centre                         | Mobile Banking Member  | Notifications grouped by app name                     |
| Authorize Production Rollout | Tyfone Support Coordination                        | FI Operations / Tyfone | Requires UAT sign-off from credit union               |
| Update Prisma Configuration  | Prisma > Settings > Push Notifications Setup     | FI Operations Admin    | Needed when migrating UAT to Production URLs          |

**Appendix: Jira Ticket Reference**

|               |                                                                                                                                              |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **Attribute** | **Detail**                                                                                                                                   |
| Ticket        | SUP-37427                                                                                                                                    |
| Summary       | Prisma Push Notification Setup                                                                                                               |
| Status        | Development Complete                                                                                                                         |
| Priority      | Medium                                                                                                                                       |
| Assignee      | Naveen Balakrishnan                                                                                                                          |
| Reporter      | Ranjini H.K                                                                                                                                  |
| Created       | April 7, 2026                                                                                                                                |
| Environment   | UAT — Validated                                                                                                                              |
| Key Finding   | Prisma Push Notification setup screen requires updating by Guillermo Winkler to reflect the latest configuration changes for Summerville FCU |
