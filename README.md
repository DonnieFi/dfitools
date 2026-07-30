# dfitools

My portable inventory of the command-line tools I use across new machines.

It is deliberately a **tool list, not a bootstrap script**: hosts have different roles, package managers, and trust requirements. Pick what fits, install it using the linked upstream instructions, and keep the version record current.

## Tool shelf

| Area | Tools |
| --- | --- |
| Terminal | [Starship](https://starship.rs), [Kitty](https://sw.kovidgoyal.net/kitty/) |
| AI & agents | [Claude Code](https://docs.anthropic.com/en/docs/claude-code), [Cursor](https://cursor.com), `agy`, [Codex CLI](https://developers.openai.com/codex/cli/), [OpenCode](https://opencode.ai), [Grok CLI](https://github.com/xai-org/grok-cli), [Ollama](https://ollama.com), [herdr](https://github.com/nickboucher/herdr), [ccusage](https://github.com/ryoppippi/ccusage) |
| Development | [GitHub CLI](https://cli.github.com), [beads](https://github.com/steveyegge/beads), [CodexBar](https://github.com/nickboucher/CodexBar), `tang`, [ruff](https://docs.astral.sh/ruff/), [uv](https://docs.astral.sh/uv/) |

The complete, versioned list—including command names and installation notes—is in [TOOLS.md](TOOLS.md).

## Use it anywhere

```bash
git clone https://github.com/DonnieFi/dfitools.git
cd dfitools
```

Then open [TOOLS.md](TOOLS.md) and install only the tools appropriate for that machine. Versions are a snapshot, not requirements: prefer the maintained upstream install instructions.

## Keeping it current

After setting up or refreshing a machine:

1. Run the version commands for the tools you installed.
2. Update [TOOLS.md](TOOLS.md) with the observed versions and any useful install notes.
3. Commit the change so the list remains a helpful record.

## Source host

| Host | Notes |
| --- | --- |
| `deba` | Debian 13 desktop — original scan source |

## Scope

This tracks standalone CLI tools. It intentionally excludes runtimes, Homebrew itself, and ordinary language libraries, with a few explicitly noted global AI CLI exceptions.
