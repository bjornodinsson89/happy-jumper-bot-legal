# Privacy Policy — Happy Jumper Bot

**Last updated:** 2026-02-20  
**Operator:** BjornOdinsson89

This Privacy Policy explains what data **Happy Jumper Bot** collects, how it is used, and your choices.

---

## 1) Summary
The Bot processes Discord identifiers and Torn API-derived information to operate features like raffles, jump sessions, approvals, and verification workflows. The Operator does **not** sell your personal data.

---

## 2) Data We Collect

### 2.1 Discord Data
Depending on usage and server configuration, the Bot may collect and store:
- Discord user ID
- Username/display name (as provided by Discord)
- Server (guild) ID
- Channel ID, role ID
- Message IDs and timestamps related to Bot workflows (entries, approvals, logs)

### 2.2 Bot Feature Data
The Bot may store:
- Raffle definitions and entry records (who entered, when, counts)
- Jump session records (host, roster, readiness/verification state, timestamps)
- Insurance requests and claim/deny actions (including who claimed)
- Server configuration settings (channels, roles, announcement toggles)
- User preferences required for correct operation (e.g., timezone, where implemented)

### 2.3 Torn API-Derived Data (Required)
The Bot requires a Torn API key and will use it to request **scoped information** needed for features such as:
- Payment verification / item-send or log verification (where used)
- Session readiness indicators (based on allowed, relevant Torn data)
- Torn identity references needed to map Discord users to Torn identities (where required)

The Bot does **not** use the Torn API to modify your Torn account (see Torn API Disclosure in this repository).

---

## 3) How We Use Data
We use collected data to:
- Provide and maintain Bot features
- Prevent abuse, fraud, and spam (verification and auditability)
- Provide audit logs for Server Admins (as part of workflows)
- Troubleshoot and improve reliability

---

## 4) Data Sharing
Data is shared only as necessary:
- With your server community when the Bot posts workflow messages into channels
- With hosting providers needed to run the Bot (e.g., database/hosting), under appropriate access controls

We do not sell personal data.

---

## 5) Retention
We retain data only as long as needed for:
- Running the Bot and maintaining workflow state
- Abuse prevention and troubleshooting
- Reasonable dispute resolution (for community workflows)

Note: messages posted into Discord channels may be retained by Discord and/or server admins even if Bot-side records are deleted.

---

## 6) Security
We use reasonable measures to protect data (least-privilege access, secret handling practices). No system is perfectly secure.

---

## 7) Your Choices and Requests
You may request:
- A copy of Bot-stored data associated with your Discord ID (where feasible)
- Deletion of Bot-stored data associated with your Discord ID (subject to retention needs and technical constraints)

To request this, contact the Operator: **BjornOdinsson89**.

---

## 8) Children
The Bot is not intended for users under the minimum age required by Discord in your region.

---

## 9) Changes
We may update this Privacy Policy from time to time. Continued use of the Bot after updates indicates acceptance of the updated Policy.
