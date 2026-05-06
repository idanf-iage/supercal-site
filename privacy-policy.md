# Privacy Policy for SuperCal

**Effective date:** 2026-04-27  
**Last updated:** 2026-05-06

## What SuperCal Does

SuperCal is a Chrome extension that adds task-management features to Google Calendar: day focus mode, content indicators, bulk event moving, and layout improvements. It enhances the Google Calendar interface directly in your browser without requiring an account or any external service.

---

## Data Accessed

SuperCal requests access to your Google Calendar data via the Google Calendar API using the OAuth2 scope `https://www.googleapis.com/auth/calendar.events`. The specific types of Google user data accessed are:

- **Event metadata:** event IDs, titles, start/end dates and times, time zones
- **Event content:** event descriptions and location fields (used only to detect whether content is present, not stored or transmitted)
- **Calendar event list:** the list of events visible in the current calendar view

This data is accessed only on-demand, only while you are actively using the extension, and only to power the features described below.

---

## Data Usage

SuperCal uses Google user data exclusively to provide its in-browser features:

| Feature | Data Used | Purpose |
|---------|-----------|---------|
| Content Indicators | Event description and location fields | Detect whether an event has a description or location so the extension can display a visual indicator |
| Bulk Move | Event IDs, start/end times, time zones | Move selected events to a different date via the Calendar API |

**SuperCal does not use Google user data for any other purpose**, including advertising, profiling, analytics, machine learning, or any purpose beyond the direct in-browser functionality described above.

All data processing happens locally within your browser. API calls are made directly from the extension's service worker to the Google Calendar API — no intermediate server is involved.

---

## Data Sharing

SuperCal does **not** share Google user data with any third party. Specifically:

- No calendar data is sent to any server owned or operated by SuperCal or its developer.
- No analytics services, advertising networks, or data brokers receive any data.
- No data is shared with other Chrome extensions or applications.

The only external communication the extension makes is direct API calls to `https://www.googleapis.com/calendar/v3/` on your behalf, using your OAuth token.

---

## Data Storage and Protection

SuperCal stores **only** your feature toggle preferences (on/off settings for each feature) in `chrome.storage.sync`. This data:

- Contains no personal information and no Google user data
- Is synced across your Chrome sessions via your Google account's built-in Chrome sync
- Is never transmitted to any server other than Chrome's built-in sync infrastructure

**OAuth tokens** are obtained via Chrome's built-in Identity API (`chrome.identity`) and are managed entirely by the browser. SuperCal never writes OAuth tokens to `chrome.storage`, `localStorage`, cookies, or any other persistent storage. Tokens are used in-memory only for the duration of a single API request.

**No Google Calendar data is ever written to disk or persistent storage** by this extension.

---

## Data Retention and Deletion

Because SuperCal does not collect or store any Google user data, there is no calendar data to retain or delete.

The only data stored by SuperCal is your feature toggle preferences in `chrome.storage.sync`. This data contains no personal information. You can delete it at any time by:

1. Uninstalling SuperCal from Chrome — this automatically clears all extension storage
2. Or clearing extension data manually via Chrome's developer tools

To request deletion of any data or for any privacy-related questions, contact: **idan.file@gmail.com**

---

## Contact

For questions about this privacy policy, contact: idan.file@gmail.com
