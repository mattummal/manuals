# Fast Node Manager

Node version manager I use.

## Installation

[Source](https://github.com/Schniz/fnm#using-a-script-macoslinux)

```
curl -fsSL https://fnm.vercel.app/install | bash
```

Then add to the end of your `~/.zshrc`:

```bash copy filename=".zshrc"
# fnm env https://github.com/Schniz/fnm
eval "$(fnm env --use-on-cd)"
```

## Usage

```bash
fnm ls

fnm install --lts

fnm use --lts

fnm install v18.12.1

fnm use v18.12.1

fnm current
```
