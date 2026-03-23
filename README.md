# Dev Control Plane (DCP) - Releases

Pre-built releases of the Dev Control Plane MCP server for [Cursor IDE](https://cursor.com/).

## Installation

1. Add to your Cursor MCP config (`~/.cursor/mcp.json`):

```json
{
  "mcpServers": {
    "dcp": {
      "command": "uvx",
      "args": [
        "--from",
        "https://github.com/dataloop-ai-apps/dcp-releases/releases/download/0.12.0/dcp_mcp-0.12.0-py3-none-any.whl",
        "dcp-mcp"
      ]
    }
  }
}
```

2. Restart Cursor.

> Replace the version in the URL with the [latest release](https://github.com/dataloop-ai-apps/dcp-releases/releases).

## What is this?

An MCP server that provides role-based AI assistance, coding guidelines search, active learning, and repo memory across your projects.

## Requirements

- [Cursor IDE](https://cursor.com/)
- Python 3.10+
- [uv](https://docs.astral.sh/uv/) (for `uvx`)
