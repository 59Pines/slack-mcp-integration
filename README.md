This repository contains the OAuth callback page for the 59 Pines Slack MCP server integration.

## Installation

Click the button below to install the Slack MCP integration:

<a href="https://slack.com/oauth/v2/authorize?client_id=137040525284.9172153638244&scope=channels:read&user_scope=channels:history,channels:read,chat:write,groups:history,groups:read,im:history,im:read,mpim:history,mpim:read,users:read&redirect_uri=https://59pines.github.io/slack-mcp-integration/slack/oauth-success.html">
  <img alt="Add to Slack" height="40" width="139" src="https://platform.slack-edge.com/img/add_to_slack.png" srcSet="https://platform.slack-edge.com/img/add_to_slack.png 1x, https://platform.slack-edge.com/img/add_to_slack@2x.png 2x" />
</a>

## Configuration

After installation, configure Cursor with your user token:

```json
{
  "mcpServers": {
    "slack": {
      "command": "npx",
      "args": ["-y", "slack-mcp-server@latest", "--transport", "stdio"],
      "env": {
        "SLACK_MCP_XOXP_TOKEN": "xoxp-your-token-here"
      }
    }
  }
}
```
