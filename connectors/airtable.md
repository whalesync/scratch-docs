# Airtable

Connect your Airtable bases to Scratch to edit and manage your content with AI.

## Authentication

Scratch supports two ways to connect to Airtable:

- **OAuth** (recommended) - Click "Connect with Airtable" and authorize access
- **API Key** - Use a personal access token from your Airtable account

<details>

<summary>How to get an API key</summary>

1. Go to [airtable.com/create/tokens](https://airtable.com/create/tokens)
2. Click **Create new token**
3. Give it a name (e.g., "Scratch")
4. Add scopes:
   - `data.records:read` - to read your records
   - `data.records:write` - to update records
   - `schema.bases:read` - to see your base structure
5. Under **Access**, add the bases you want to use with Scratch
6. Click **Create token**
7. Copy the token (starts with `pat`)

</details>

## What you can sync

- Airtable bases and tables
- Records and field values

## Getting started

1. Go to **Data Sources** in Scratch
2. Click **Add Connection** and select Airtable
3. Authorize access or enter your API key
4. Select the bases and tables you want to work with
5. Create a Workbook from your connection

## Supported field types

### Text fields

| Field Type | Support |
|------------|---------|
| Single line text | ✅ Read/Write |
| Long text | ✅ Read/Write |
| Rich text | ✅ Read/Write |
| Email | ✅ Read/Write |
| URL | ✅ Read/Write |
| Phone number | ✅ Read/Write |
| Barcode | ➡️ Read Only |

### Number fields

| Field Type | Support |
|------------|---------|
| Number | ✅ Read/Write |
| Percent | ✅ Read/Write |
| Currency | ✅ Read/Write |
| Rating | ✅ Read/Write |
| Duration | ✅ Read/Write |
| Count | ➡️ Read Only |
| Auto number | ➡️ Read Only |

### Date fields

| Field Type | Support |
|------------|---------|
| Date | ✅ Read/Write |
| Date and time | ✅ Read/Write |
| Created time | ➡️ Read Only |
| Last modified time | ➡️ Read Only |

### Select fields

| Field Type | Support |
|------------|---------|
| Single select | ✅ Read/Write |
| Multiple select | ✅ Read/Write |

### Relationship fields

| Field Type | Support |
|------------|---------|
| Link to another record | ✅ Read/Write |
| Lookup | ➡️ Read Only |

### Other fields

| Field Type | Support |
|------------|---------|
| Checkbox | ✅ Read/Write |
| Attachments | ✅ Read/Write |
| Collaborator | ✅ Read/Write |
| Formula | ➡️ Read Only |
| Rollup | ➡️ Read Only |
| Created by | ➡️ Read Only |
| Last modified by | ➡️ Read Only |
| Button | ➡️ Read Only |
