# tiny-chess-01 — v6c

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/arshamax16/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/arshamax16/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB Python chess engine for the make.fun tiny-chess gauntlet. It searches with alpha-beta over a 0x88 board, a depth-preferred transposition table, quiescence on captures and checks, and a history heuristic with killer moves for ordering. Late moves are reduced aggressively (2 plies when more than 8 legal moves remain), which buys deeper effective search inside the same 65,000-node budget. Everything is deterministic: the node budget, not a clock, decides each move.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 -P -s main.py
```

`main.py` is the packed engine (source: `engine_v6c.py`, compressed with `makefun compress`).

---

<sub>Entered on [make.fun](https://make.fun/?ref=pstpm556&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
