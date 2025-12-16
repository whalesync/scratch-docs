# Webflow

Connect your Webflow CMS collections to Scratch to edit and manage content with AI.

## Authentication

Scratch supports two ways to connect to Webflow:

- **OAuth** (recommended) - Click "Connect with Webflow" and authorize access
- **API Key** - Use a site API token from your Webflow project settings

<details>

<summary>How to get a Webflow API key</summary>

1. Go to your Webflow dashboard
2. Open the site you want to connect
3. Click **Site settings** (gear icon)
4. Go to the **Apps & Integrations** tab
5. Scroll down to **API Access**
6. Click **Generate API token**
7. Copy the token

Note: Site API tokens have access to that specific site only. For multiple sites, use OAuth instead.

</details>

## What you can sync

- CMS collections and items
- Collection item fields and content

## Getting started

1. Go to **Data Sources** in Scratch
2. Click **Add Connection** and select Webflow
3. Authorize access or enter your API key
4. Select the site and collections you want to work with
5. Create a Workbook from your connection

## Supported field types

| Field Type | Support |
|------------|---------|
| Plain text | ✅ Read/Write |
| Rich text | ✅ Read/Write |
| Number | ✅ Read/Write |
| Switch (boolean) | ✅ Read/Write |
| Date/time | ✅ Read/Write |
| Email | ✅ Read/Write |
| Phone | ✅ Read/Write |
| Link | ✅ Read/Write |
| Video link | ✅ Read/Write |
| Option (select) | ✅ Read/Write |
| Color | ✅ Read/Write |
| Reference | ✅ Read/Write |
| Slug | ✅ Read/Write |
| Is draft | ➡️ Read Only |
| Is archived | ➡️ Read Only |
| Last published | ➡️ Read Only |
| Last updated | ➡️ Read Only |
| Created on | ➡️ Read Only |

### Rich text format

Rich text fields can be edited as HTML or Markdown. Scratch handles the conversion automatically.
