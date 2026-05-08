<div align="center">

# Cli Builder Ai MCP

**CLI Builder AI MCP Server**

[![PyPI](https://img.shields.io/pypi/v/meok-cli-builder-ai-mcp)](https://pypi.org/project/meok-cli-builder-ai-mcp/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![MEOK AI Labs](https://img.shields.io/badge/MEOK_AI_Labs-MCP_Server-purple)](https://meok.ai)

</div>

## Overview

CLI Builder AI MCP Server
CLI tool generation and parsing utilities powered by MEOK AI Labs.

## Tools

| Tool | Description |
|------|-------------|
| `generate_argparse` | Generate Python argparse CLI boilerplate code. |
| `generate_click` | Generate Python Click CLI boilerplate code. |
| `parse_help_text` | Parse CLI help text output into structured command/option data. |
| `generate_manpage` | Generate a man page in troff format. |

## Installation

```bash
pip install meok-cli-builder-ai-mcp
```

## Usage with Claude Desktop

Add to your Claude Desktop MCP config (`claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "cli-builder-ai": {
      "command": "python",
      "args": ["-m", "meok_cli_builder_ai_mcp.server"]
    }
  }
}
```

## Usage with FastMCP

```python
from mcp.server.fastmcp import FastMCP

# This server exposes 4 tool(s) via MCP
# See server.py for full implementation
```

## License

MIT © [MEOK AI Labs](https://meok.ai)
