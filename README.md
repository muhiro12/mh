# mh — Minimal helper CLI for local iOS workflows

`mh` is a single‑file shell script that wraps common Git + Xcode
operations (build/test, Codex PR handling, branch sync, self‑update, …).
The exact sub‑commands evolve quickly; consult `mh -h` for the current list.

## Quick start

```bash
# 1. Download and install to ~/bin
mkdir -p ~/bin
curl -fsSL https://raw.githubusercontent.com/muhiro12/mh/refs/heads/main/mh \
  -o ~/bin/mh && chmod 755 ~/bin/mh

# 2. (Optional) install GitHub CLI — required for Codex / PR features
mh -i          # wraps 'brew install gh'

# 3. Show available commands
mh -h
```

That’s it — keep the script up to date at any time:

```bash
mh -u          # fetch latest version from GitHub
```

---

*For detailed usage run `mh -h` or read the inline comments in `mh` itself.*
