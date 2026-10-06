# 🎲 DICE RACE 100 — 3D Multiplayer Dice Game

3D dice game (Three.js) with online multiplayer via room code (PeerJS P2P — no server to host).

## How to run
Just double-click `index.html` — or serve it:
```
npx serve .
```
Internet needed for the Three.js + PeerJS CDNs.

## Rules (as requested)
1. **Free play for now** — betting chips are parked until development is complete. Just race to 100 for glory.
2. **Only 4 rerolls per turn** — ROLL, then click a die to HOLD it and reroll the other. BANK to keep your turn score. Rerolls reset each turn.
3. **First to 100 wins** — banked points accumulate; first to 100+ takes the pot.

Extras: doubles = +5 bonus, snake eyes (1+1) = BUST (lose turn score).

## Modes
- 🤖 **Solo vs AI** — practice against the computer
- 👥 **Local 2P** — pass-and-play on one device
- 🌐 **Create Room** — generates a random 5-letter code (e.g. `K7Q2M`). Share it with a friend.
- 🔑 **Join Room** — enter the code to connect across networks (P2P via PeerJS cloud, works on different servers/networks).

## How online works
1. Player 1 clicks **Create Room** → gets a code.
2. Player 2 clicks **Join Room**, enters the code + name → **Connect**.
3. Host sets the bet → **START GAME**. Dice rolls sync live on both screens.
