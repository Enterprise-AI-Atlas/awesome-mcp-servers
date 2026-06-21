# Contributing

Contributions are welcome. Please read this guide before opening a pull request.

## What belongs in this list

This registry is for Model Context Protocol (MCP) servers that let AI agents, coding assistants, and MCP clients interact with external services, data sources, and platforms. Acceptable entries include:

- MCP servers that expose a product, API, or protocol to MCP clients.
- Official vendor servers and reference implementations.
- Well-maintained community servers with clear documentation.
- Curated collections or registries that help discover MCP servers.

## What does **not** belong

- General SDK documentation or tutorials that are not MCP-server oriented.
- Closed-source or paywalled-only tools with no public documentation.
- Duplicate entries.
- Abandoned or unmaintained projects.

## Quality bar

Every submission must be:

1. **Publicly accessible** — open source or publicly documented.
2. **Actively maintained** — last meaningful commit or release within the last 12 months (exceptions for official vendor reference repos).
3. **Documented** — a real README with setup or install instructions.
4. **Correctly categorized** — placed under the domain it primarily targets.
5. **Honestly labeled** — use the `Official` or `Community` badge.

## Entry format

Use this pattern:

```markdown
- **[Name](URL)** `Official` — One-sentence description.
  - Install: `command here`
```

If there is no install command, omit the install line.

## Category sections

The README is organized by **domain or service category**. New category sections are allowed only if they contain at least five entries.

## Pull request process

1. Fork the repository.
2. Add your entry in the correct category section.
3. Run `./scripts/validate-links.sh` and fix any broken links or anchors.
4. Open a pull request with a clear description of the server and why it fits.

One resource per pull request is preferred.
