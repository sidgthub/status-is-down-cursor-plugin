# Status Is Down for Cursor

Connect Cursor to Status Is Down's read-only outage intelligence.

Status Is Down covers 13,500+ services. MCP results depend on available records and evidence; not every service has complete historical or geographic data.

## Capabilities

Six read-only tools let you:
- Check current service status
- Explore daily outage-report history, up to 31 days
- Explore geographic report patterns where evidence is available
- Compare provider status evidence with community reports
- Investigate spikes in report activity
- Find a service in the monitored catalog

A report spike is not necessarily a confirmed outage. Tools do not change monitoring settings, send alerts, or perform remediation.

## Connect to Cursor

Add this entry to your Cursor MCP configuration, merging it with any existing servers:

```json
{
  "mcpServers": {
    "status-is-down": {
      "url": "https://statusisdown.com/api/mcp"
    }
  }
}
```

Use Cursor's authentication flow to sign in with your Status Is Down business account and authorize read-only access. Access can be revoked through SID's MCP workspace.

Availability depends on Cursor's MCP support, account plan and administrator settings.

## Example prompts

- "Check Cloudflare's current status using Status Is Down."
- "Show Slack's available daily outage reports for the past week."
- "What recent geographic outage evidence is available for Spotify?"
- "Does Slack show a recent spike in community reports?"

## Plans and credits

SID MCP is separate from SID monitoring subscriptions.

MCP Free includes 500 credits each UTC calendar month. Status queries cost 10 credits and may be repeated within the balance. Each other function may be used once per month at its listed cost.

Paid plans and optional credit packs are purchased on statusisdown.com, not through this plugin. Invalid inputs, SID errors and no-data results are not charged.

See the product page for current pricing, limits and connection instructions.

## Links

- [Product and documentation](https://statusisdown.com/business/mcp )
- [MCP workspace](https://statusisdown.com/business/mcp/connect )
- [Privacy policy](https://statusisdown.com/privacy )
- [Terms of use](https://statusisdown.com/terms )
- [Support](https://statusisdown.com/business#general-contact )

## License

This repository contains plugin configuration and documentation, not the hosted MCP server source.

The configuration and documentation are MIT-licensed. The hosted Status Is Down service is operated by SID Monitor Pte Ltd and remains subject to its own terms. The SID logo remains its owner's trademark.
