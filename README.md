# Customable Claude Plugins

Extended Claude Code plugins maintained by [Customable](https://customable.de).

## Installation

Add the marketplace to Claude Code:

```
/plugin marketplace add https://git.customable.host/customable/claude-plugins.git
```

Then install plugins:

```
/plugin install claude-mem@customable-plugins
```

## Available Plugins

### claude-mem

**Persistent memory across Claude Code sessions**

Claude-Mem automatically captures observations, decisions, and discoveries from your coding sessions and injects relevant context into future sessions.

**Features:**
- Automatic observation extraction via Claude Agent SDK
- Vector search with Qdrant for semantic retrieval
- Web viewer UI at `localhost:37777`
- MCP server for natural language memory queries
- Multi-platform support: Claude Code, Cursor, OpenCode

**Documentation:** [mem.customable.host](https://mem.customable.host)

## Attribution

The `claude-mem` plugin is based on [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem), originally created by [@thedotmack](https://github.com/thedotmack). This fork includes extended features:

- Qdrant vector database support (in addition to Chroma)
- OpenCode platform adapter
- Enhanced Web UI with console logs viewer
- Export/Import API endpoints
- Network binding configuration (WORKER_BIND)
- Various bug fixes and improvements

We are grateful to thedotmack for creating this excellent tool and making it open source under the MIT license.

## License

MIT License - See individual plugin repositories for details.
