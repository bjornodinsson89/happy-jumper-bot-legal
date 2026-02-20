# Torn API Disclosure & Disclaimer — Happy Jumper Bot

**Last updated:** 2026-02-20  
**Operator:** BjornOdinsson89

This document explains (1) what the Torn API is, (2) what the Bot uses it for, (3) what the Bot does *not* do, and (4) important limitations.

---

## 1) What the Torn API Is (High-Level)
The **Torn API** is a web-based interface provided by Torn that allows authorized users to retrieve certain game-related data programmatically using an API key. The API is commonly used to read information such as user details, logs, items, faction/member data, travel status, and other game state that Torn exposes through its API endpoints.

Your Torn API key is a credential. Anyone who has it may be able to access the data that key is permitted to access.

---

## 2) Torn API Key Requirement (No Optional Mode)
**Happy Jumper Bot requires a Torn API key to operate.** The Bot uses your key to request **scoped information** necessary for its features.

You agree:
- You will only provide an API key you are authorized to use.
- You understand Torn API rate limits, outages, and changes can affect Bot operation.
- You understand the Bot can only read what the Torn API allows for your key’s access/permissions.

---

## 3) What the Bot Uses the Torn API For
The Bot uses the Torn API strictly for **read-only retrieval** of information needed to operate server workflows, such as:

### A) Verification & Audit Workflows
- Verifying whether a user performed a required in-game action (for example, checking a relevant log category where supported)
- Correlating entries/purchases with verification signals to reduce fraud and improve fairness

### B) Happy Jump Session Coordination
- Pulling only the relevant Torn data needed to:
  - Determine readiness indicators (e.g., cooldown/conditions as implemented)
  - Display session-relevant status for participants
  - Assist hosts/admins with accurate roster state

### C) Identity & Reference Data
- Resolving Torn identifiers needed to map server workflows (e.g., pairing a Discord user to a Torn user where required)
- Fetching item metadata needed for display/validation (when applicable)

The Bot is designed to use **only the minimum Torn API data required** to provide these features.

---

## 4) What the Bot Does NOT Do (Important)
The Bot does **not**:
- Automate gameplay actions on your behalf
- Perform in-game clicks, attacks, trades, purchases, or movement
- Send items, money, or messages inside Torn
- Modify or write to Torn account state

The Bot operates **within Discord** and uses Torn API calls only to **read** data that Torn exposes to your key.

---

## 5) Data Accuracy, Limits, and Availability
- **Accuracy:** Torn API responses may be delayed, incomplete, or inconsistent with in-game views.
- **Rate Limits:** Torn enforces rate limiting. The Bot may cache or throttle requests to stay within limits.
- **Outages/Changes:** Torn may change endpoints, data fields, permissions, or availability at any time. This can break features without notice.

---

## 6) Key Handling and Security Notes
- Treat your Torn API key like a password.
- Do not share your key publicly.
- If you believe your key is compromised, rotate/regenerate it in Torn and update it in the Bot.

The Operator uses reasonable practices to protect secrets and minimize stored sensitive information, but no system is perfectly secure.

---

## 7) Contact
Questions about this disclosure should be directed to the Operator: **BjornOdinsson89**.
