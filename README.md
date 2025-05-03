# Discord Suggestion Bot

A powerful Discord bot that allows server members to submit suggestions that can be voted on, approved, or rejected by moderators. The bot provides a complete suggestion management system with embeds, voting, and notification features.

## Features

- 📝 User-friendly suggestion submission system
- 👍👎 Upvote and downvote functionality
- ✅❌ Approval/rejection system for moderators
- 📊 Suggestion statistics and tracking
- 🔔 Rich embed notifications for suggestion status updates

## Setup Guide

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher)
- A Discord Bot Token ([Discord Developer Portal](https://discord.com/developers/applications))
- A Discord server with appropriate permissions

### Installation

1. Clone or download this repository

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure the bot:
   - Edit the `.env` file and add your Discord bot token
   - Edit the `config.json` file with your Discord server's channel and role IDs

4. Set up your Discord server:
   - Create a channel for suggestions
   - Create a channel for logs
   - Create a role for approvers/moderators
   - Enable Developer Mode in Discord (User Settings > App Settings > Advanced)
   - Right-click on channels and roles to copy their IDs

5. Start the bot:
   ```bash
   node index.js
   ```
   or
   ```bash
   npm start
   ```

## Usage

### For Users

- Send a message in the suggestions channel to create a suggestion
- Use 👍 and 👎 buttons to vote on suggestions

### For Moderators

- Click the "Accept" or "Reject" buttons on suggestions to approve or reject them
- Provide a reason when accepting or rejecting
- Use slash commands for additional management:
  - `/suggestion info [id]` - Get detailed information about a suggestion
  - `/suggestion stats` - View suggestion statistics
  - `/suggestion voters [id] [type]` - See who voted on a suggestion

## Customization

You can customize the bot's appearance and behavior by modifying the `index.js` file. Look for the embed creation sections to change colors, titles, and other visual elements.

## Support

If you need help setting up or using the bot, feel free to join our Discord server for support.