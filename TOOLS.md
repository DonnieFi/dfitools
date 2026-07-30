# CLI tools

Last scanned from **deba** (Debian 13). CLIs only — no brew, node, npm, or Python libraries (except a few global AI CLIs noted below).

## Terminal

| Tool | Version | Install notes |
|------|---------|---------------|
| [starship](https://starship.rs) | 1.25.0 | `curl -sSf https://starship.rs/install.sh \| sh` |
| [kitty](https://sw.kovidgoyal.net/kitty/) | 0.47.2 | Linux installer / distro package |

## AI / agent CLIs

| Tool | Version | Install notes |
|------|---------|---------------|
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code) (`claude`) | 2.1.152 | Anthropic installer |
| [Cursor](https://cursor.com) (`cursor`) | — | Desktop app + CLI shim |
| [cursor-agent](https://cursor.com) | 2026.07.09 | Bundled with Cursor agent |
| `agy` | 1.1.8 | Agent CLI in `~/.local/bin` |
| [Codex CLI](https://developers.openai.com/codex/cli/) (`codex`) | 0.146.0 | OpenAI installer → `~/.local/bin` |
| [OpenCode](https://opencode.ai) (`opencode`) | 1.17.18 | `~/.opencode/bin` |
| [Grok CLI](https://github.com/xai-org/grok-cli) (`grok`) | 0.2.93 | Grok installer → `~/.grok/bin` |
| [herdr](https://github.com/nickboucher/herdr) | 0.7.1 | Binary in `~/.local/bin` |
| [ccusage](https://github.com/ryoppippi/ccusage) | — | `npm i -g ccusage` (global AI CLI exception) |
| [Ollama](https://ollama.com) (`ollama`) | 0.30.6 | Official installer / local model runner |


## Dev / workflow

| Tool | Version | Install notes |
|------|---------|---------------|
| [GitHub CLI](https://cli.github.com) (`gh`) | — | `apt install gh` or [official install](https://github.com/cli/cli#installation) |
| [beads](https://github.com/steveyegge/beads) (`bd`, `beads`) | 1.0.4 | Release binary → `~/.local/bin` |
| [CodexBar](https://github.com/nickboucher/CodexBar) (`codexbar`, `CodexBarCLI`) | 0.41.0 | Homebrew formula `codexbar` (or manual install) |
| `tang` | 0.2.9 | `tang-multiverse`; agent-work continuation CLI in `~/.local/bin` |
| [ruff](https://docs.astral.sh/ruff/) | 0.15.14 | `pip install --user ruff` or `uv tool install ruff` |
| [uv](https://docs.astral.sh/uv/) | 0.5.9 | `curl -LsSf https://astral.sh/uv/install.sh \| sh` |
