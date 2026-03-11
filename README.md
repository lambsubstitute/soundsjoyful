# Wix Website Project

Project for helping with the soundjoyful Wix website.

## Sounds Joyful — Workplace Wellbeing Content

Ready-to-use website copy for the Sounds Joyful workplace wellbeing extension:

| File | Contents |
|------|----------|
| `sounds-joyful/01-workplace-wellbeing-overview.md` | Main landing page — hero, intro, three experience cards, social impact |
| `sounds-joyful/02-reset-experience.md` | The Reset Experience (45–60 min) page |
| `sounds-joyful/03-connection-experience.md` | The Connection Experience (3-hour) page |
| `sounds-joyful/04-immersion-retreat.md` | The Immersion Retreat (full day) page |
| `sounds-joyful/05-why-sounds-joyful.md` | "Why Sounds Joyful" section + HR pitch |
| `sounds-joyful/06-science-of-music-wellbeing.md` | Optional Science of Music page |
| `sounds-joyful/07-wix-implementation-guide.md` | Step-by-step Wix implementation guide |

---

## Wix MCP Server

This workspace is configured with the Wix MCP server, which enables:

- **Documentation search** — Wix Design System, REST API, SDK, Build Apps, Headless docs
- **Site management** — List sites, make API calls, create/update records
- **Code assistance** — Get full API schemas and step-by-step flow instructions

## Getting Started

1. Open this folder in Cursor (`File → Open Folder → WixWebsite`)
2. Restart Cursor if the MCP was just added (MCP servers load at startup)
3. Start asking for help with the Wix site — the AI will have access to Wix tools

## Optional: API Key Authentication

For tools like `ListWixSites`, `CallWixSiteAPI`, and `ManageWixSite`, you may need to authenticate. Update `.cursor/mcp.json` to add headers:

```json
{
  "mcpServers": {
    "wix-mcp": {
      "type": "http",
      "url": "https://mcp.wix.com/mcp",
      "headers": {
        "Authorization": "<YOUR WIX API KEY>",
        "wix-account-id": "<YOUR ACCOUNT ID>"
      }
    }
  }
}
```

Get API keys from the [Wix Developer Center](https://dev.wix.com/).

## Prerequisites

- Node.js 19.9.0 or higher
