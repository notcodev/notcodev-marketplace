# Notcodev Marketplace

Personal Claude Code plugin marketplace. Plugins are hosted in external repositories.

## Installation

Add this marketplace to Claude Code:

```bash
/plugin marketplace add notcodev/notcodev-marketplace
```

## Available Plugins

### Claude Weeek

**Description:** Claude Code plugin for the [WEEEK](https://weeek.net) task tracker — direct read/write access to projects, boards, tasks, and comments via MCP.

**Categories:** MCP, Task Management, Productivity

**Install:**
```bash
/plugin install claude-weeek@notcodev-marketplace
```

**What you get:**
- 12 tools — 7 read (projects, boards, columns, tasks, comments) + 5 write (create/update/move/complete tasks, post comments)
- Read/write split — reads can be auto-approved while writes stay gated
- Token auth via `WEEEK_API_TOKEN` env var, never logged
- Safe defaults — paginated list tools (default 20, max 50) stay under the 25k token MCP limit
- No delete operations — v1 intentionally omits destructive endpoints

**Requirements:** Node.js >= 20, WEEEK API token

**Repository:** https://github.com/notcodev/claude-weeek

---

## Marketplace Structure

```
notcodev-marketplace/
├── .claude-plugin/
│   └── marketplace.json       # Plugin catalog
└── README.md                  # This file
```

## Support

- **Issues**: https://github.com/notcodev/notcodev-marketplace/issues

## License

Marketplace metadata: MIT License

Individual plugins: See respective plugin licenses
