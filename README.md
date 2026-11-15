# makefun-tiny-chess-02

A tiny chess engine in at most 4,096 bytes of Python, written for the
make.fun tiny-chess-01 bounty. `main.py` is the whole engine: a 0x88 board,
negamax with alpha-beta and PVS, a Zobrist transposition table, killers,
MVV-LVA and history ordering, a check extension, quiescence search, and
iterative deepening to a fixed 50,000-node budget. The evaluation is
material plus piece-square tables with a tapered king table and a tempo
bonus. It plays the house gauntlet through the env at `MAKEFUN_ENV_URL`.

The readable source is `dev/engine.py` (kept out of this snapshot so the
repository stays inside the size caps); `main.py` is its LZMA-packed form,
made with `makefun compress`.
