# Torn API Disclosure and Disclaimer

**Last updated:** 2026-02-20

This document explains what the Torn API is, what it typically provides, how this Bot uses it (if enabled), what it does **not** do, and important disclaimers.

> **Not affiliated:** This Bot is an independent community tool and is **not affiliated with, endorsed by, or sponsored by Torn**.

---

## 1. What the Torn API is

The **Torn API** is a programmatic interface provided by Torn that allows approved requests to retrieve certain game/account information. In general, APIs like this are used by tools to read data (and in some cases submit actions if the provider supports it). The Torn API is typically accessed using an **API key** associated with a Torn account.

Common categories of information that an API like Torn’s can expose (depending on endpoint and key permissions) include:

- Basic account and profile information
- Faction information (e.g., members, wars, status)
- Logs (e.g., activity records, item transfer logs where supported)
- Travel and status-related information
- Item metadata (names, IDs, images) and other reference data

**Important:** The exact fields available, rate limits, and permissions are defined by Torn and can change over time.

---

## 2. Your API key and permissions

If you choose to enable Torn API features:

- You must use a key you are authorized to use.
- You should grant **only** the permissions required for the Bot features you want.
- Treat your API key like a password. Do not share it publicly.

If the Bot asks for specific permissions, it is because those endpoints require them to function.

---

## 3. What this Bot uses the Torn API for

When Torn API integration is enabled, the Bot may use Torn API calls for the following purposes (depending on the features you use and how your Server is configured):

### 3.1 Verification workflows
The Bot may retrieve log or transaction-like information to help **verify** that an in-game action occurred (for example, confirming that a particular item was sent to a particular account ID).

Typical examples include:

- Checking recent logs for item sends that match a configured requirement (e.g., a particular item ID and recipient ID)
- Extracting the relevant log entry and posting a verification summary into a configured admin/announcement channel

### 3.2 Roster/readiness helpers
The Bot may retrieve limited account status information to help a Server coordinate events, such as:

- Whether a participant appears ready (based on configured criteria)
- Whether certain cooldown/state conditions appear satisfied (as available from the API)

### 3.3 Reference data
The Bot may retrieve item metadata used for display:

- Item IDs / names / image URLs
- Normalized naming for common items (to reduce spelling/case issues)

---

## 4. What this Bot does **not** do with the Torn API

Even when integration is enabled, the Bot is designed **not** to:

- Perform gameplay actions on your behalf (e.g., attacks, travel, purchases, trades)
- Send items or money for you
- Modify your Torn account
- Bypass Torn restrictions, limits, or policies

The Bot’s Torn API usage is focused on **reading data to support community coordination and verification**.

---

## 5. Data handling and storage notes

Depending on implementation, the Bot may:

- Store **only what is needed** to operate features (e.g., verification results, timestamps, and minimal identifiers)
- Avoid storing API keys in plaintext, and instead store them in a protected form (e.g., encryption) or avoid persistence where possible

No system can guarantee absolute security. You use the integration at your own risk.

---

## 6. Rate limits, failures, and accuracy

The Torn API may enforce:

- Rate limits (requests per minute/hour)
- Availability windows or temporary outages
- Permission restrictions that block certain endpoints

Because of this:

- Verification can fail even when a user acted correctly (e.g., logs delayed or unavailable)
- Data may be incomplete or stale
- The Bot may temporarily disable certain features to respect rate limits

---

## 7. Disclaimer

- The Bot is provided **as-is** and **as-available**.
- The Bot does not guarantee the accuracy, completeness, or timeliness of Torn API data.
- You are responsible for ensuring your usage complies with Torn’s rules, policies, and API terms.
- Server Admins are responsible for how verification and coordination results are used within their Server.

---

## 8. Questions

If you have questions about what endpoints are used or what permissions are required for a feature, contact the Bot operator via the official support method advertised in the Bot’s documentation or official Server.
