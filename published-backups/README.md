# Published Backups

This folder stores point-in-time copies of the schema markup that is actually live on the Astra Dental Centre website.

## Why keep backups here?

The schema files in the other folders (dentist, faq, service, etc.) are the working source / templates. This folder is for the EXACT JSON-LD that has been deployed and verified live, so there is a record of what is on each page at a given time.

## Naming convention

Use the page slug and date, for example:

- `homepage_2025-01-15.json`
- `dentist-langley_2025-01-15.json`
- `invisalign-service_2025-01-15.json`

## How to capture a backup

1. Open the live page and view source (or use the Rich Results Test).
2. Copy the full JSON-LD block exactly as it appears on the page.
3. Save it here with the page slug and the date it was verified live.
4. Note the date you confirmed it with the Google Rich Results Test.

## Notes

- Keep one backup per page per significant change, not one per day.
- Do not store any secrets, API keys, or tracking IDs in these files.
- If review counts or ratings change, capture a fresh backup so the record stays accurate.
