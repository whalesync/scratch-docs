# FAQ

## General

### What is Scratch?

Scratch is an AI editor for published content. It connects to your content platforms (WordPress, YouTube, Notion, etc.), lets you work with AI to edit your content in bulk, and publishes approved changes back to the source.

### Is my content safe?

Yes. Scratch works on a copy of your content in a temporary sandbox. Your live content is never touched until you explicitly review, approve, and click Publish. You see every change as a diff before anything goes live.

### Do you store my content?

Content is stored temporarily while you work on it. Once you push your approved changes and delete the workbook, your content is removed from our servers. Your content stays yours.

### What AI models can I use?

Scratch supports multiple AI models through OpenRouter. Free users have access to 5 models. Pro users can use any model and bring their own OpenRouter API key.

## Connections

### Why use OAuth instead of an API key?

OAuth is recommended because:
- It's more secure (no keys to manage or accidentally expose)
- Permissions are scoped to exactly what Scratch needs
- You can revoke access anytime from the service's settings

### Can I connect multiple accounts?

On the Pro plan, you get one account per service. On the Max plan, you can connect multiple accounts per service - useful for agencies managing client content.

### Why can't I see my database/collection?

For Notion: Make sure you've shared the database with your Scratch integration. Go to your database in Notion, click Share, and add your integration.

For other services: Check that your API key or OAuth connection has the necessary permissions to access the content.

## Editing

### How do I undo AI changes?

All AI suggestions appear as diffs that you can accept or reject. Click the X on any suggestion to reject it. You can also click "Reset" to reload fresh content from the source.

### Can I edit the same content in Scratch and the source?

We recommend avoiding this. Scratch works on a snapshot of your content. If you edit the source while working in Scratch, you may overwrite those changes when you publish. Either finish your Scratch edits first, or reset to pull fresh content.

### Why is the AI making wrong suggestions?

Try these fixes:
- Be more specific in your prompt
- Add context via prompt assets (style guides, examples)
- Use a more capable model for complex tasks
- Filter to a smaller set of records so the AI can focus

## Publishing

### What happens when I publish?

Scratch sends your approved changes back to the source platform via its API. Only fields you've modified and accepted are updated - unchanged content is left alone.

### Can I preview before publishing?

Yes. The publish dialog shows exactly which records and fields will be updated, with a diff of the changes. Review this carefully before confirming.

### What if publishing fails?

If a publish fails, Scratch will show you which records failed and why. Common causes are permission issues, API rate limits, or validation errors from the platform. Your workbook retains the changes so you can fix the issue and try again.
