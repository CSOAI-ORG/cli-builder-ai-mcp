# CLI Builder AI MCP Server

> By [MEOK AI Labs](https://meok.ai) — Generate CLI tool boilerplate (argparse, Click) and parse help text

## Installation

```bash
pip install cli-builder-ai-mcp
```

## Usage

```bash
python server.py
```

## Tools

### `generate_argparse`
Generate Python argparse CLI boilerplate code with arguments and subcommands.

**Parameters:**
- `program_name` (str): CLI program name
- `description` (str): Program description
- `arguments` (list[dict]): Arguments with keys: name, type, help, required, default, choices
- `subcommands` (list[dict]): Optional subcommands

### `generate_click`
Generate Python Click CLI boilerplate code with command groups and options.

**Parameters:**
- `program_name` (str): CLI program name
- `description` (str): Program description
- `commands` (list[dict]): Commands with keys: name, help, options

### `parse_help_text`
Parse CLI help text output into structured command/option data.

**Parameters:**
- `help_text` (str): CLI help text output (from --help)

### `generate_manpage`
Generate a man page in troff format with options, examples, and author info.

**Parameters:**
- `program_name` (str): Program name
- `description` (str): Program description
- `version` (str): Version string
- `synopsis` (str): Usage synopsis line
- `options` (list[dict]): Options with keys: flag, description
- `examples` (list[dict]): Examples with keys: command, description
- `author` (str): Author name

## Authentication

Free tier: 50 calls/day. Upgrade at [meok.ai/pricing](https://meok.ai/pricing) for unlimited access.

## License

MIT — MEOK AI Labs
