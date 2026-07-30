# Terminal setup

The tools in [TOOLS.md](TOOLS.md) are useful on their own. These small configuration choices make them feel like a coherent workstation.

## At a glance

| Layer | Current choice |
| --- | --- |
| Shell | Bash with history append, completion, and useful PATH entries |
| Prompt | [Starship](https://starship.rs), with directory and Git branch context |
| Terminal | [Kitty](https://sw.kovidgoyal.net/kitty/) with [Catppuccin Mocha](https://github.com/catppuccin/kitty) |
| Font | [Nerd Fonts](https://www.nerdfonts.com/) for prompt glyphs |
| Remote shell | Kitty's SSH kitten (`kitty +kitten ssh`) |

## Bash

Add the following after your PATH setup in `~/.bashrc`:

```bash
# Preserve and share shell history across sessions.
HISTCONTROL=ignoreboth
shopt -s histappend checkwinsize

# Enable Bash completion when the package is installed.
if [ -f /usr/share/bash-completion/bash_completion ]; then
  . /usr/share/bash-completion/bash_completion
fi

# Starship prompt.
eval "$(starship init bash)"

# Preserve Kitty's terminal capabilities over SSH.
alias ssh="kitty +kitten ssh"
```

Keep secrets out of `~/.bashrc`: source them from a private file with restrictive permissions, or use a dedicated secrets manager. Never commit them here.

## Starship prompt

Save this as `~/.config/starship.toml` for a minimal prompt that shows the working directory and current Git branch:

```toml
format = "$directory$git_branch$character"

[directory]
style = "bold blue"
truncation_length = 3
truncate_to_repo = true

[git_branch]
symbol = " "
style = "bold purple"

[character]
success_symbol = "[❯](bold green)"
error_symbol = "[❯](bold red)"
```

## Kitty and fonts

Kitty uses Catppuccin Mocha, 92% background opacity, and **JetBrainsMono Nerd Font**. A Nerd Font is important because Starship and many developer tools use glyphs outside an ordinary monospace font. FiraCode Nerd Font is also installed as an alternative.

To switch Kitty to FiraCode Nerd Font:

```conf
# ~/.config/kitty/kitty.conf
font_family FiraCode Nerd Font
font_size 12.0
include current-theme.conf
background_opacity 0.92
```

Download or install fonts from [Nerd Fonts](https://www.nerdfonts.com/font-downloads), then restart Kitty.

## Kitty theme

Install the [Catppuccin Kitty Mocha theme](https://github.com/catppuccin/kitty/blob/main/themes/mocha.conf) as `~/.config/kitty/current-theme.conf`, then include it from `kitty.conf`:

```conf
include current-theme.conf
```

## What stays local

Do not copy machine-specific absolute paths, API tokens, model credentials, or SSH private keys into this repository. Keep this document focused on portable behavior and public configuration.
