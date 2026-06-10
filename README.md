# nakaba-lab Scoop bucket

A [Scoop](https://scoop.sh) bucket for **[`sshm`](https://github.com/nakaba-lab/ssh-manager-tui)** — a Windows-first terminal UI for browsing, editing, and connecting to the SSH hosts in your `~/.ssh/config`.

## Install

```powershell
scoop bucket add nakaba-lab https://github.com/nakaba-lab/scoop-bucket
scoop install sshm-tui
```

This installs the **`sshm`** command (Windows x64). Then just run:

```powershell
sshm
```

## Notes

- The app is distributed on crates.io and here as **`sshm-tui`** (the bare `sshm` name was already taken on both crates.io and Scoop's `main` bucket by unrelated tools); the installed **binary/command is `sshm`**.
- Manifests live in [`bucket/`](bucket/). Each version tracks the upstream [GitHub releases](https://github.com/nakaba-lab/ssh-manager-tui/releases) via `checkver` + `autoupdate`.

## Update / uninstall

```powershell
scoop update sshm-tui
scoop uninstall sshm-tui
```
