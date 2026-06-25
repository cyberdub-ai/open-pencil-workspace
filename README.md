# open-pencil-workspace

Design workspace powered by [OpenPencil](https://github.com/open-pencil/open-pencil) — open-source Figma alternative with AI and MCP support.

## Setup (cyberdub-ai .44 server)

### MCP server (headless, Claude Code)

```bash
npm install -g @open-pencil/mcp
bash ~/bin/open-pencil-on.sh   # enable in Claude Code
# restart Claude Code
bash ~/bin/open-pencil-off.sh  # disable when done
```

Config: `~/.claude/mcp-extras/open-pencil.json`  
Workspace root: `~/projects/open-pencil-workspace`

### CLI

```bash
npm install -g @open-pencil/cli
openpencil analyze colors design.fig
openpencil analyze typography design.fig
openpencil variables design.fig
```

### Web

No self-host needed — P2P, no backend:  
https://app.openpencil.dev

## MCP tools

100+ design tools accessible via `mcp__open-pencil__*` in Claude Code.  
Creates, modifies, exports `.pen` and `.fig` documents headlessly.

## Workspace files

| File | Project | Description |
|------|---------|-------------|
| — | — | — |

## Notes

- v0.13.2 (2026-05-30), active development, not production-ready
- RTX 3090 not relevant — rendering is client-side WASM (Skia)
- Collaboration: WebRTC P2P, share via `app.openpencil.dev/share/<room>`
