# <img src="../.gitbook/assets/wordpress.svg" alt="" data-size="line"> WordPress

Connect your WordPress site to Scratch to edit and manage blog posts with AI.

## Authentication

WordPress uses application password authentication:

- **Username** - Your WordPress admin username
- **Application Password** - Generate one in WordPress under Users → Security
- **Site URL** - Your WordPress site's REST API endpoint

## What you can sync

- Blog posts and their content
- Post titles, excerpts, and metadata

## Getting started

1. Go to **Data Sources** in Scratch
2. Click **Add Connection** and select WordPress
3. Enter your username, application password, and site URL
4. Create a Workbook from your connection

## Setting up application passwords

1. Log into your WordPress admin
2. Go to **Users** → **Profile**
3. Scroll to **Application Passwords**
4. Enter a name (e.g., "Scratch") and click **Add New**
5. Copy the generated password

## Supported field types

WordPress fields are discovered dynamically from your site's REST API. Common fields include:

| Field | Support |
|-------|---------|
| Title | ✅ Read/Write |
| Content | ✅ Read/Write |
| Excerpt | ✅ Read/Write |
| Slug | ✅ Read/Write |
| Status | ✅ Read/Write |
| Date | ✅ Read/Write |
| Categories | ✅ Read/Write |
| Tags | ✅ Read/Write |
| Featured image | ✅ Read/Write |
| Author | ✅ Read/Write |
| ID | ➡️ Read Only |
| Modified date | ➡️ Read Only |
| Link | ➡️ Read Only |

### Advanced Custom Fields (ACF)

If your site uses ACF, those fields are also supported and appear as additional columns in your workbook.

### Content format

Post content can be edited as HTML or Markdown. Scratch handles the conversion automatically.
