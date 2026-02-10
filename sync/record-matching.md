# Record Matching

When a sync runs, Scratch pairs records between your source and destination based on a **matching field** — a field that has the same value on both sides.

## How it works

You select a field mapping to use as your matching field. This could be a field such as:

- Title
- Email address
- Name
- An explicit ID you've set up in your tables

The matching field must be included in your sync's field mappings.

When the sync runs, for each record in the source:

1. Scratch looks for a record in the destination with the same matching field value
2. If one is found, changes sync to that record
3. If none is found, a new record is created in the destination
4. If multiple matching records are found, the record is skipped to avoid creating duplicates

## Choosing a matching field

Pick a field that:

- Has **unique values** — no duplicates on either side
- Has **real values** — not blank or empty on any records you want to sync

Records where the matching field is blank or not unique will not be synced.

If you can't find a field that meets these criteria, reach out to us at support@scratch.md — we're curious to hear about your data and needs.
