# Sanjhai's Gmail Cleanup Assistant

A free n8n workflow to keep your Gmail inbox clean by automatically deleting spam, promotional, social, and trash emails daily at 2:00 AM. It sends a summary report via Telegram.

## Features
- Deletes emails from Spam, Promotions, Social, and Trash categories.
- Processes up to 250 emails per category per run.
- Sends a Telegram notification with a summary report.
- Runs daily at 2:00 AM (customizable).

## Files
- [**Sanjhai_s_Gmail_Cleanup_Assistant.json**](./Sanjhai_s_Gmail_Cleanup_Assistant.json): The n8n workflow file.
- [**GmailCleanupGuide.pdf**](./GmailCleanupGuide.pdf): Detailed setup guide.

## How to Use
1. Download the JSON file and import it into your n8n instance (Workflows > Import Workflow).
2. Follow the setup instructions in the [GmailCleanupGuide.pdf](./GmailCleanupGuide.pdf).
3. Configure Gmail OAuth2 and Telegram credentials.
4. Test and activate the workflow.

## Prerequisites
- An n8n instance (self-hosted or cloud): [n8n.io](https://n8n.io/).
- Gmail API OAuth2 credentials: [Google Cloud Console](https://console.cloud.google.com/).
- Telegram bot and chat ID: [Telegram BotFather](https://core.telegram.org/bots#creating-a-new-bot).

## Warning
- **Permanent Deletion**: The workflow permanently deletes emails, especially from Trash. Test with a small `limit` (default: 250 emails per category) to avoid data loss.
- **Gmail API Limits**: Be aware of Gmail API quotas (e.g., 250 read/write operations per second).

## License
Free to use, modify, and share under the [MIT License](LICENSE).

## Support
For help, contact Sanjhai at [sanjhaiprakash18@gmail.com](mailto:sanjhaiprakash18@gmail.com) or visit the [n8n Community Forum](https://community.n8n.io/).

## Feedback
Share your thoughts on X with `#n8n` or star this repository if you find it useful!
