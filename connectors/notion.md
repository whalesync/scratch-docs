# Notion

Connect your Notion databases to Scratch to edit and manage your content with AI.

## Authentication

Scratch supports two ways to connect to Notion:

- **OAuth** (recommended) - Click "Connect with Notion" and authorize access
- **API Key** - Create an integration in Notion and paste your API key

<details>

<summary>How to get an API key</summary>

1. Go to [notion.so/my-integrations](https://www.notion.so/my-integrations)
2. Click **New integration**
3. Give it a name (e.g., "Scratch")
4. Select the workspace you want to connect
5. Click **Submit**
6. Copy the **Internal Integration Secret** (starts with `ntn_`)
7. **Important**: Share your databases with the integration:
   - Open each database you want to use in Scratch
   - Click **Share** in the top right
   - Click **Invite**
   - Search for your integration name and select it

</details>

## What you can sync

- Notion databases and their properties
- Page content within database items

## Getting started

1. Go to **Data Sources** in Scratch
2. Click **Add Connection** and select Notion
3. Authorize access or enter your API key
4. Select the databases you want to work with
5. Create a Workbook from your connection

## Supported field types

| Field Type | Support |
|------------|---------|
| Title | ✅ Read/Write |
| Rich Text | ✅ Read/Write |
| Number | ✅ Read/Write |
| Select | ✅ Read/Write |
| Multi-select | ✅ Read/Write |
| Status | ✅ Read/Write |
| Date | ✅ Read/Write |
| Checkbox | ✅ Read/Write |
| URL | ✅ Read/Write |
| Email | ✅ Read/Write |
| Phone | ✅ Read/Write |
| Relation | ✅ Read/Write |
| Formula | ➡️ Read Only |
| Rollup | ➡️ Read Only |
| Created time | ➡️ Read Only |
| Created by | ➡️ Read Only |
| Last edited time | ➡️ Read Only |
| Last edited by | ➡️ Read Only |
| People | ➡️ Read Only |
| Files | ➡️ Read Only |

## Page Content

Notion pages contain block-based content. Scratch converts this to Markdown for editing and syncs changes back as blocks.

### Supported block types

| Block Type | Support |
|------------|---------|
| Paragraph | ✅ Read/Write |
| Heading 1 | ✅ Read/Write |
| Heading 2 | ✅ Read/Write |
| Heading 3 | ✅ Read/Write |
| Bulleted list | ✅ Read/Write |
| Numbered list | ✅ Read/Write |
| To-do list | ✅ Read/Write |
| Toggle | ✅ Read/Write |
| Quote | ✅ Read/Write |
| Code | ✅ Read/Write |
| Callout | ✅ Read/Write |
| Divider | ✅ Read/Write |
| Table | ✅ Read/Write |
| Image | ✅ Read/Write |
| Video | ✅ Read/Write |
| Audio | ✅ Read/Write |
| File | ✅ Read/Write |
| PDF | ✅ Read/Write |
| Bookmark | ✅ Read/Write |
| Embed | ✅ Read/Write |
| Equation | ✅ Read/Write |
| Table of contents | ✅ Read/Write |
| Breadcrumb | ✅ Read/Write |
| Column layout | ✅ Read/Write |
| Synced block | ✅ Read/Write |
| Child page | ➡️ Read Only |
| Link to page | ➡️ Read Only |

### Rich text formatting

Inline formatting is preserved:

- **Bold**, *italic*, ~~strikethrough~~, `code`
- Underline and text colors
- Hyperlinks
