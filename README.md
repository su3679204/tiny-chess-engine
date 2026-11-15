# Tiny Chess Engine (4 KB)

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/su3679204/tiny-chess-engine/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/su3679204/tiny-chess-engine/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact chess engine in a single `main.py` (<= 4,096 bytes, Python 3.13
standard library only). The file unpacks an lzma-compressed payload and
execs it: 0x88 board, alpha-beta search with transposition table,
quiescence search, null-move pruning, MVV-LVA + TT-move ordering, and
sunfish piece-square tables. Search is to a fixed node count (50,000
nodes/move), so every trial is deterministic and replay-identical.

## Run it

```sh
MAKEFUN_ENV_URL=<env url> python3 -P -s main.py
```

## Files

- `main.py` — the whole engine (4,070 bytes).
- `LICENSE` — MIT.

---

<sub>Entered on [make.fun](https://make.fun/?ref=fyqrs5z4&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
