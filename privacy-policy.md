# Privacy Policy for SuperCal

**Effective date:** 2026-04-27

## What SuperCal Does

SuperCal is a Chrome extension that adds task-management features to Google Calendar: day focus mode, content indicators, bulk event moving, and layout improvements.

## Data We Access

SuperCal requests access to your Google Calendar events via the Google Calendar API (OAuth2 scope: `calendar.events`). This access is used solely to:

- Read event details (to detect whether events have descriptions or locations)
- Move events between days when you use the bulk-move feature

## Data We Store

SuperCal stores only your feature toggle preferences (on/off settings for each feature) in `chrome.storage.sync`. This data:

- Contains no personal information
- Is synced across your Chrome sessions via your Google account
- Is never transmitted to any server other than Chrome's built-in sync infrastructure

## Data We Do NOT Collect

- We do not collect, store, or transmit your calendar event data to any external server.
- We do not use analytics, tracking, or telemetry.
- We do not share any data with third parties.

## OAuth Token Handling

OAuth tokens are obtained via Chrome's Identity API and are managed entirely by the browser. SuperCal never stores OAuth tokens in extension storage or transmits them outside of requests to the Google Calendar API.

## Contact

For questions about this privacy policy, contact: idan.file@gmail.com
