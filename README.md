# nakaba-lab Scoop bucket

A [Scoop](https://scoop.sh) bucket for nakaba-lab's Windows terminal tools:

- **[`sshm`](https://github.com/nakaba-lab/ssh-manager-tui)** — a terminal UI for browsing, editing, and connecting to the SSH hosts in your `~/.ssh/config`.
- **[`wslm`](https://github.com/nakaba-lab/wsl-manager-tui)** — a terminal UI to manage WSL distributions: lifecycle, shells, live VM memory/CPU, export/import, and `.wslconfig`/`wsl.conf` editing.

## Install

```powershell
scoop bucket add nakaba-lab https://github.com/nakaba-lab/scoop-bucket
scoop install sshm-tui   # installs the `sshm` command
scoop install wslm       # installs the `wslm` command
```

Install only what you need, then run `sshm` or `wslm`.

## Notes

- `sshm` is distributed on crates.io and here as **`sshm-tui`** (the bare `sshm` name was already taken on both crates.io and Scoop's `main` bucket by unrelated tools); the installed **binary/command is `sshm`**.
- Manifests live in [`bucket/`](bucket/). Each version tracks the upstream GitHub releases via `checkver` + `autoupdate`.

## Update / uninstall

```powershell
scoop update sshm-tui
scoop update wslm
scoop uninstall sshm-tui
scoop uninstall wslm
```
