# Privacy Policy

**Effective Date:** 23 May 2026  
**Last Updated:** 23 May 2026  
**Bot:** DankAssistant  
**Operator:** DankAssistant Team

---

## 1. Introduction

This Privacy Policy explains what data DankAssistant ("the Bot", "we", "us") collects, how it is used, and your rights regarding that data. By using the Bot, you agree to the collection and use of information as described in this policy.

---

## 2. Data We Collect

We collect and store the following categories of data, tied to your Discord User ID:

### 2.1 Account & Identity
| Data | Purpose |
|------|---------|
| Discord User ID | Primary identifier for all stored data |
| Username | Display in leaderboards and audit logs |
| Privacy acceptance timestamp | Record of consent |

### 2.2 User Settings & Preferences
| Data | Purpose |
|------|---------|
| Reminder preferences (types enabled) | Deliver scheduled reminders |
| User settings (key-value pairs) | Persist feature toggles (e.g., energy drink, vote reminders) |
| Announcement read status | Avoid re-showing dismissed announcements |

### 2.3 Reminder Data
| Data | Purpose |
|------|---------|
| Active reminders (type, channel, target time, scope) | Schedule and deliver timed notifications |
| Reminder usage counts | Track reminder delivery statistics |

### 2.4 Donation Tracking
| Data | Purpose |
|------|---------|
| Donation totals per configuration | Leaderboard rankings and threshold role assignments |
| Donation ledger entries (amount, note, timestamp) | Audit trail for donation history |

### 2.5 Voting
| Data | Purpose |
|------|---------|
| Vote streak (current, longest, total votes, last vote time) | Streak tracking and vote perks |
| Vote audit log (operation, before/after state) | Transparency and dispute resolution |

### 2.6 Work Shift Tracking
| Data | Purpose |
|------|---------|
| Daily work shift records (date, job name, success/fail counts) | Progress display and promotion tracking |

### 2.7 Premium & Subscription
| Data | Purpose |
|------|---------|
| Subscription status and period dates | Manage premium access |
| Premium slot assignments (guild, source, expiry) | Activate server perks |
| Payment transaction records | Billing history |

### 2.8 Moderation
| Data | Purpose |
|------|---------|
| Blacklist status (if applicable) | Enforce bot-level bans |

---

## 3. Data We Do NOT Collect

- **Message content** — We do not read or store the content of your messages. The Bot only processes messages from specific bots (e.g., Dank Memer) for auto-tracking features you opt into.
- **Voice data** — We do not join voice channels or process audio.
- **DMs** — We do not read your direct messages. DMs from the Bot are one-way notifications.
- **Browsing/activity outside Discord** — We have no access to anything outside the Discord platform.
- **IP addresses** — We do not log your IP address.

---

## 4. How Data Is Used

Your data is used exclusively to:

1. **Provide Bot features** — reminders, donation tracking, leaderboards, vote streaks, work shift tracking, and premium access.
2. **Personalize your experience** — respecting your settings and preferences.
3. **Maintain service integrity** — enforcing blacklists and preventing abuse.

We do **not**:
- Sell your data to third parties
- Use your data for advertising
- Share your data with other users (except public leaderboard rankings which display usernames)
- Train AI/ML models on your data

---

## 5. Data Storage & Security

- All data is stored in a **PostgreSQL database** hosted on secured infrastructure.
- Frequently accessed data is cached in **Redis** with appropriate TTLs.
- Access to production systems is restricted to authorized operators only.
- All connections use encrypted transport (TLS).

---

## 6. Data Retention

| Data Type | Retention |
|-----------|-----------|
| Active reminders | Until triggered or cancelled |
| Donation records | Indefinite (while guild uses the Bot) |
| Vote streaks | Indefinite (while account exists) |
| Vote audit log | Last 50 entries retained |
| Work shift records | Last 30 days |
| Subscription data | Indefinite (for billing history) |
| Blacklist entries | Until expiry or manual removal |
| All user data | **Deleted immediately upon request** via `/privacy deletemydata` |

---

## 7. Your Rights

You have the following rights at any time by using the `/privacy` command:

### 7.1 Right to Access (`/privacy requestmydata`)
Request a full export of all data we store about you. The Bot will provide a JSON file containing every piece of your data.

### 7.2 Right to Deletion (`/privacy deletemydata`)
Request permanent deletion of **all** your data. This action:
- Removes all records from every table listed in Section 2
- Cancels active premium subscriptions and slots
- Is **irreversible** — your leaderboard positions, streaks, and history cannot be recovered
- Takes effect immediately upon confirmation

### 7.3 Right to Withdraw Consent
You may stop using the Bot at any time. If you delete your data, the Bot will no longer process any information about you.

---

## 8. Consent & Privacy Gate

- You must accept this Privacy Policy (via `/privacy accept`) before using any Bot features.
- A **3-day grace period** is provided after policy deployment or updates to allow continued access while you review the policy.
- After the grace period, unaccepted users are blocked from all Bot features except `/privacy`.
- Reminder notifications will include a nudge if you have not yet accepted.

---

## 9. Data Shared with Third Parties

| Third Party | Data Shared | Purpose |
|-------------|-------------|---------|
| Discord | Interactions, message content sent by Bot | Required for Bot operation |
| top.gg | None (they send vote events to us) | Vote webhook reception |
| Payment processor | User ID, subscription details | Premium billing |

We do not share your personal data with any other third parties.

---

## 10. Guild (Server) Data

Server administrators who configure the Bot (donation configs, channel settings, etc.) should be aware:
- Guild configuration data is tied to the **guild ID**, not individual users.
- Donation leaderboard data contains user IDs and usernames of members who donated.
- When a user deletes their data, their entries are removed from guild leaderboards.

---

## 11. Children's Privacy

The Bot is not intended for users under the age of 13, consistent with Discord's Terms of Service. We do not knowingly collect data from children under 13.

---

## 12. Changes to This Policy

- We may update this Privacy Policy from time to time.
- When the policy version changes, you will be required to re-accept within a new 3-day grace period.
- Continued use after the grace period requires acceptance of the updated policy.
- Major changes will be announced via the Bot's announcement system.

---

## 13. Contact

For privacy concerns, data requests, or questions about this policy:
- Use the `/privacy` command in Discord
- Contact the Bot operators via the support server

---

## 14. Legal Basis for Processing (GDPR)

For users in the European Economic Area (EEA), our legal basis for processing your data is:
- **Consent** — You explicitly accept this policy before features are available.
- **Legitimate interest** — Maintaining service integrity (blacklists, abuse prevention).

---

## 15. California Residents (CCPA)

California residents have additional rights:
- **Right to Know** — Covered by `/privacy requestmydata`
- **Right to Delete** — Covered by `/privacy deletemydata`
- **Right to Non-Discrimination** — We do not discriminate against users who exercise their privacy rights
- **No Sale of Personal Information** — We do not sell your personal information to any party
