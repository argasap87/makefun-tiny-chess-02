# makefun-tiny-chess-02

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/argasap87/makefun-tiny-chess-02/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/argasap87/makefun-tiny-chess-02/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in at most 4,096 bytes of Python, written for the
make.fun tiny-chess-01 bounty. `main.py` is the whole engine: a 0x88 board,
negamax with alpha-beta and PVS, a Zobrist transposition table, killers,
MVV-LVA and history ordering, a check extension, quiescence search, and
iterative deepening to a fixed 50,000-node budget. The evaluation is
material plus piece-square tables with a tapered king table and a tempo
bonus. It plays the house gauntlet through the env at `MAKEFUN_ENV_URL`.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=1ae1r9cj&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>

The readable source is `dev/engine.py` (kept out of this snapshot so the
repository stays inside the size caps); `main.py` is its LZMA-packed form,
made with `makefun compress`.
