# SharePoint

Cursor plugin that connects agents to [Microsoft SharePoint](https://www.microsoft.com/microsoft-365/sharepoint) through Cursor's remote [Model Context Protocol](https://modelcontextprotocol.io/) server.

Search sites, browse document libraries, and read list items in the signed-in Microsoft account.

## Install

1. Open **Cursor Settings → Plugins**.
2. Search for **SharePoint**.
3. Click **Install**, then complete the Microsoft sign-in prompt.

Or run `/add-plugin sharepoint` in chat.

## MCP

```json
{
  "mcpServers": {
    "sharepoint": {
      "type": "http",
      "url": "https://api.cursor.com/rest-mcp/sharepoint/mcp"
    }
  }
}
```

Auth is OAuth 2.0 against Microsoft (Entra ID). Cursor prompts for Microsoft sign-in when the plugin connects.

## Docs

- SharePoint API (Microsoft Graph): https://learn.microsoft.com/en-us/graph/api/resources/sharepoint
- Microsoft Graph overview: https://learn.microsoft.com/en-us/graph/overview

Logo is the official Microsoft SharePoint product icon from Microsoft's Fluent brand icon CDN, placed on a white tile with padding so it reads well in the Cursor UI:
https://res-1.cdn.office.net/files/fabric-cdn-prod_20240411.001/assets/brand-icons/product/svg/sharepoint_48x1.svg

## License

MIT
