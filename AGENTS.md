# Documentation project instructions

## About this project

- Documentation site for **Relay** (https://github.com/termdx/Relay), built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- The product's own design specs live in `Relay/.specs/` — they are the
  source of truth for how anything works; never contradict them
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

- "Workspace" — a self-hosted Relay instance managed by the runtime (not "project")
- "Project" — a client's engagement inside Relay (not "workspace")
- "Client" — the agency's customer, who uses the portal
- "Owner" / "founder" — the Relay user (desktop app), never "admin"
- "Knowledge base" — the per-project source of truth, not "vector store"
- "Portal" — the client-facing web app; "desktop" — the founder control plane

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Only document shipped behavior — the status tables in `Relay/.specs/`
  say what is shipped vs planned

## Content boundaries

- Don't document internal admin features (runtime daemon RPC surface,
  outbox internals) — user-facing surfaces only
- Don't document planned features as if they exist (Temporal, Google
  Calendar/S3 adapters are planned)
- No secrets, tokens, or real credentials in examples — use placeholders
