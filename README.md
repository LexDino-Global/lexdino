# LexDino: Israeli Law Research

Source-backed research in Israeli law, in Hebrew and English. The plugin connects Claude to the LexDino corpus of Israeli court rulings and statutes: it searches the corpus, reads the exact passages an answer relies on, resolves citations and verifies quotations against the text that was read.

Scope: Israeli law only. Foreign and international law are not covered.

## What you need

An existing Louis account at [louis-ai.net](https://louis-ai.net). You sign in once, on Louis's own consent page; consent grants tool access only. Nothing is charged through Claude: payment happens only on the Louis website.

## Install

In claude.ai, Claude Desktop and Cowork, add the plugin from the directory, or add the connector `https://mcp.lexdino.com/mcp` under Settings → Connectors, then sign in with your Louis account.

In Claude Code:

```text
/plugin install lexdino --marketplace LexDino-Global/lexdino
```

## What it does

- **Search** Israeli rulings and statutes with Hebrew or English queries.
- **Read** the passages an answer relies on, so every claim points at its paragraph.
- **Resolve citations** and **verify quotations** against the text that was read.
- **Report coverage**: what was searched and read, and where the research is partial.
- **Export** a research record as HTML, Markdown or DOCX.
- **Managed research** (optional): runs when your existing subscription covers it.

## What the plugin runs, sends and stores

- The plugin contains no executable code: one remote MCP server entry (`.mcp.json`) and one Markdown Skill.
- Claude sends your research queries, citation strings, quotations to verify and research identifiers to `https://mcp.lexdino.com/mcp`, operated by LexDino. Nothing is sent to any other destination.
- LexDino stores research sessions, the passages read, usage records and the sign-in grant. See the [privacy policy](https://louis-ai.net/privacy) and [terms of use](https://louis-ai.net/terms).
- The service provides legal information and sources, not legal advice, and does not create a lawyer-client relationship.

Support: [louis-ai.net/contact](https://louis-ai.net/contact) or office@louis-ai.net.
