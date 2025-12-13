# ZSH Configuration

ZSH configurations using [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)

## Theme

I use oh-my-zsh for the [installation](https://github.com/spaceship-prompt/spaceship-prompt#-installation)

```bash copy filename=".zshrc"
ZSH_THEME="spaceship"
```

## Plugins

```bash copy filename=".zshrc"
plugins=(
    git
    autojump
    yarn
    gh
    zsh-syntax-highlighting
    zsh-autosuggestions
)
```

## Top 25 Zsh Aliases Demonstration

A curated list of handy Zsh aliases for faster navigation, git operations, and dev workflow.

---

### **Navigation Aliases**

| Alias | Command | Description |
|-------|---------|-------------|
| `=` | `cd -` | Go to previous directory |
| `1` | `cd +1` | Go 1 directory forward in stack |
| `2` | `cd +2` | Go 2 directories forward |
| `d` | `fasd -d` | Quickly jump to frequently used directories |
| `zz` | `fasd_cd -d -i` | Interactive directory jump |

---

### **Git Aliases**

| Alias | Command | Description |
|-------|---------|-------------|
| `g` | `git` | Base git command |
| `gs` | `git status` | Check git status |
| `gco` | `git checkout` | Checkout a branch or file |
| `gca` | `git commit --verbose --all` | Commit all changes verbosely |
| `gp` | `git push` | Push commits to remote |

---

### **Python / Dev Aliases**

| Alias | Command | Description |
|-------|---------|-------------|
| `python` | `python -m IPython --no-confirm-exit` | Start IPython REPL |
| `pip` | `python -m pip` | Use pip for package management |
| `pytest` | `python -m pytest -vv` | Run tests with verbose output |
| `mypy` | `python -m mypy` | Run type checking |
| `ipdb` | `python -m ipdb` | Debug Python scripts interactively |

---

### **Utilities / Tools**

| Alias | Command | Description |
|-------|---------|-------------|
| `_` | `sudo` | Run commands as superuser |
| `la` | `ll -A` | List all files with details |
| `df` | `df -kh` | Show disk usage in human-readable format |
| `du` | `du -kh` | Show directory sizes |
| `topc` | `htop -s PERCENT_CPU` | Monitor CPU usage interactively |
| `topm` | `htop -s PERCENT_MEM` | Monitor memory usage interactively |
| `watchgpu` | `watch --color -n0.2 "gpustat --color || gpustat"` | Watch GPU usage live |
| `o` | `open` | Open files or directories (macOS) |
| `e` | `${(z)VISUAL:-${(z)EDITOR}}` | Open editor (VISUAL or EDITOR env) |
| `v` | `vim` | Open Vim/nvim editor |
| `tmux` | `tmux-wrapper` | Start or attach tmux session |

---

> These aliases are sourced from a curated Zsh setup and showcase how **navigation, git workflow, Python development, and system monitoring** can be made faster in the terminal.
---
