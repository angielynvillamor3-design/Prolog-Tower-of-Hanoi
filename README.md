# Tower-of-Hanoi


## Features

- Three towers (A, B, C) on a wooden platform, with colorful gradient rings
- **AUTO SOLVE** using the recursive Tower of Hanoi algorithm (A to C, with B as the spare)
- **PAUSE** and **RESUME** from the exact current move
- **RESET** that safely cancels any running animation
- Choose 3 to 8 disks; the minimum number of moves (2^n - 1) is calculated automatically
- Speed control: Slow, Normal, Fast, Very Fast (can be changed while solving)
- Three-stage ring animation: lift, move across, lower
- Web Audio sound effects for pick up, drop and puzzle completion, with a Sound ON/OFF toggle
- Live display of moves, minimum moves, elapsed time, status and progress
- "PUZZLE SOLVED!" screen with total moves, minimum moves and solving time
- Responsive layout for desktop, tablet and mobile

## The Rules

1. Move only one disk at a time.
2. Only move the top disk of a tower.
3. Never place a larger disk on top of a smaller one.

## How the Solver Works

To move `n` disks from tower A to tower C using tower B as the spare:

1. Move the top `n - 1` disks from A to B.
2. Move the largest disk from A to C.
3. Move the `n - 1` disks from B to C.

The fewest possible moves is `2^n - 1` (7 for 3 disks, 255 for 8 disks).
