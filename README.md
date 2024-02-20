# URL Shortening Service & Slack Bot Integration

This project consists of two components: a URL shortening service and a Slack bot. The URL shortening service allows users to shorten long URLs, while the Slack bot provides a convenient interface for users to shorten URLs directly within Slack.

## URL Shortening Service

The URL shortening service is responsible for shortening long URLs into shorter, more manageable ones.

- Gihub link: https://github.com/Chandan2812/url-shorten
- Deployed link: https://urlshorten-rzcr.onrender.com/

## Slack Bot

The Slack bot provides a convenient interface for users to shorten URLs directly within Slack channels.

### Deployment

The Slack bot has been deployed and is integrated into your Slack workspace.

## Setup

To set up and run the URL shortening service and Slack bot locally, follow these steps:

1. Clone the repository for the URL shortening service:
   ```bash
   # Clone the repository:
   git clone <url-shorten-repo-url>
   
   # navigate to the repository:
   cd url-shorten
   
   # Install dependencies:
   npm install
   
   # .env file
   PORT:8000
   
   # Start the server:
   node index.js
   ```

1. Clone the repository for slack bot:
   ```bash
   # Clone the repository:
   git clone <slack-url-shortener repo link>
   
   # navigate to the repository:
   cd slack-url-shortener
   
   # Install dependencies:
   npm install
   
   # .env file
   PORT:3000
   SLACK_BOT_TOKEN: Slack bot user token.
   SLACK_SIGNING_SECRET: Slack app signing secret.
   SLACK_APP_TOKEN: Slack app token.
   
   # Start the server:
   node index.js
   ```


## Slack Bot

The Slack bot listens for commands in Slack channels and provides shortened URLs upon request.

1. **Invite the Slack bot to your workspace.**

2. In any Slack channel, use the following command to shorten a URL:
   ```bash
   /shorturl <long-url> # Replace <long-url> with the URL you want to shorten.
