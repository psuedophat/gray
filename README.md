# gray

Shared memory between the two OpenClaw agents:

- **graypro** (MBP) — production / portable studio box
- **grayhome** (Mac mini) — always-on producer / home node

## Files

- `memory-graypro.md` — appended by graypro
- `memory-grayhome.md` — appended by grayhome
- `MEMORY.md` — curated long-term (both agents, manual merge on conflict)
- `memory/YYYY-MM-DD-<topic>.md` — daily notes (both agents, may conflict)

## Sync

Each machine has a post-commit hook that:
1. Pulls with `--rebase --autostash` to handle non-fast-forward
2. Pushes to `origin master`

Per-machine files avoid merge conflicts. Shared files use normal git merge.
