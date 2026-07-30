# Configuration profiles

This page records the small, host-specific choices that make the tools in [TOOLS.md](TOOLS.md) feel at home. It complements the portable defaults in [SETUP.md](SETUP.md); do not put secrets, API tokens, private paths, or SSH keys here.

## `kiritsuke` — laptop

| Layer | Configuration |
| --- | --- |
| Shell | Bash; Starship initializes near the end of `~/.bashrc`, after Debian's default `PS1` setup |
| Prompt | Custom Starship format: username, hostname, directory, Git branch, and prompt character |
| Prompt styling | Nerd Font username glyph (`󰒍`) with Catppuccin-inspired colors |
| Terminal | Kitty with JetBrainsMono Nerd Font |
| Theme | Catppuccin Mocha |
| Remote SSH | `ssh` aliases to `kitty +kitten ssh` |
| Agent sessions | Moving from tmux to herdr; tmux is intentionally not part of the inventory |

The default Debian prompt remains in `.bashrc`, but it is harmless: `eval "$(starship init bash)"` replaces it for interactive shells.

### Starship shape

The laptop prompt intentionally shows enough identity and context to make multiple terminal windows obvious:

```text
󰒍 user@host  ~/project  branch  ❯
```

It relies on a Nerd Font for the leading glyph. Keep the configured terminal font in sync with the selected Starship symbols.

## `deba` — desktop

| Layer | Configuration |
| --- | --- |
| Prompt | Minimal Starship prompt: directory, Git branch, and prompt character |
| Terminal | Kitty with Catppuccin Mocha, 92% background opacity, and JetBrainsMono Nerd Font |
| Setup reference | [SETUP.md](SETUP.md) |

## Profile checklist

When documenting another host, capture the user-visible choices—not installation noise:

- Shell and prompt initialization order.
- Prompt segments and any required glyph font.
- Terminal emulator, font, and theme.
- Useful integrations such as Kitty SSH.
- Intentional workflow choices, such as a session tool migration.

Never commit tokens, private hostnames, private filesystem paths, credentials, or SSH material.
