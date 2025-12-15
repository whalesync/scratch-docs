# Getting started

## Welcome to Scratch

Welcome to an early look at a new way of working with content. This guide skips the fluff and gets straight to what matters: putting these tools to work.

### The core principle: a safe sandbox for live data

Scratch works by creating a temporary, isolated copy of your live data. The AI agent only ever interacts with this safe copy.

No changes are ever made to your live data until you explicitly review, approve, and click _Publish_.

This architecture puts a human-in-the-loop by design. You can experiment with powerful AI edits, knowing your original source is untouched until you give the final command.

### Getting started quickly

1. Connect: Click on _Data sources_ to link a live data source (Notion, YouTube, etc.).
2. Create: Open that connection and create a new _Workbook_.
3. Edit: Open the _Workbook_ and start giving the AI instructions.
4. Reset: Want to start over? Click _Download_ to refresh the content from the live connection.

### Key concepts for powerful editing

#### Work at the right context level

You can operate on your entire content library or on a single piece of content. The AI has access to both views:

* Library View: See all your content in a list. From here, you can ask the AI to perform broad tasks like categorizing records, generating summaries for multiple items, or even creating new records based on the context of the entire library.
* Single-Record View: Focus on a single piece of content for deep, detailed edits.

#### Accelerate the AI-human workflow

These tools are designed to make the "AI suggests, you approve" loop as fast and efficient as possible.

* Provide lasting context with prompt assets. Add reusable instructions, style guides, or content from URLs (.md, sitemaps, etc.) to the chat. The AI will use this context for its tasks, ensuring consistency and accuracy.
* Choose the right AI model. Select a fast, lightweight model for simple tasks like tagging, or a more powerful model for complex writing and editing.
* Filter with precision. Use natural language or SQL queries to instantly filter records and give the AI a focused set of data to work on.
* Review changes instantly. The UI shows all AI suggestions as string-level diffs, so you can see exactly what changed at a glance.
* Approve or reject. Accept or discard suggestions for a single cell, an entire record, or the whole library.
* Make surgical edits. Use precise tools for targeted changes without needing the AI to rewrite the whole text:
  * Find and replace: For targeted substitutions.
  * Append: To add content to the end of a field.
  * Insert: Use `@@` to mark the exact spot for new content.
* Stay in control: You can stop an agent loop at any time if it's not doing what you want.

#### Navigate like a pro with keyboard shortcuts

* Move around the library: Use the keyboard arrow keys.
* Sort columns: Use `[` and `]` to sort by the currently selected column.
* Edit cells: In the record view, press `Enter` to open/edit a cell and `Esc` to close it.
