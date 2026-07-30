<div align="center">

# dfitools

### A small, portable shelf of command-line tools worth keeping nearby.

[![Tool inventory](https://img.shields.io/badge/purpose-tool%20inventory-5B5BD6?style=flat-square)](TOOLS.md)
[![Platform](https://img.shields.io/badge/source-Debian%2013-A81D33?style=flat-square&logo=debian&logoColor=white)](TOOLS.md)
[![GitHub last commit](https://img.shields.io/github/last-commit/DonnieFi/dfitools?style=flat-square&label=last%20updated)](https://github.com/DonnieFi/dfitools/commits/main)

</div>

`dfitools` is the curated list I use when setting up a new machine: the terminal, AI, and development CLIs that have earned a spot in my workflow.

It is intentionally **not** an installer. Machines have different roles, package managers, and security boundaries. This is the useful middle ground: a portable, versioned reference with upstream links and notes, ready to copy from wherever you are.

> **Looking for the complete list?** Open **[TOOLS.md](TOOLS.md)** for command names, observed versions, and install notes.

## On the shelf

| | Category | A few highlights |
| :-: | --- | --- |
| `>_` | **Terminal** | [Starship](https://starship.rs) · [Kitty](https://sw.kovidgoyal.net/kitty/) |
| `✦` | **AI & agents** | [Claude Code](https://docs.anthropic.com/en/docs/claude-code) · [Codex CLI](https://developers.openai.com/codex/cli/) · [Cursor](https://cursor.com) · [OpenCode](https://opencode.ai) · [Ollama](https://ollama.com) · [Grok CLI](https://github.com/xai-org/grok-cli) · `agy` |
| `⌘` | **Development** | [GitHub CLI](https://cli.github.com) · [beads](https://github.com/steveyegge/beads) · [CodexBar](https://github.com/nickboucher/CodexBar) · `tang` · [ruff](https://docs.astral.sh/ruff/) · [uv](https://docs.astral.sh/uv/) |

## Take it with you

```bash
git clone https://github.com/DonnieFi/dfitools.git
cd dfitools
```

Then browse [TOOLS.md](TOOLS.md), follow the upstream instructions for the tools that fit the machine, and move on. The recorded versions are a useful snapshot—not a mandate to install old software.

## Keep the shelf tidy

When a new tool proves useful, or you refresh a machine:

1. Check its installed version.
2. Add it to [TOOLS.md](TOOLS.md), with its command, upstream link, and a note that will help Future You install it again.
3. Update the README highlights if it belongs on the front page.
4. Commit and push.

## Ground rules

| Included | Deliberately excluded |
| --- | --- |
| Standalone CLIs that support daily work | Shells and core OS utilities |
| Desktop-app CLI shims when they are genuinely useful | Runtimes and package managers themselves |
| A few global AI CLIs, explicitly noted | Ordinary language libraries |

## Origin

| Source host | Snapshot |
| --- | --- |
| `deba` | Debian 13 desktop |

---

<div align="center"><sub>Install less. Keep the good stuff close.</sub></div>
