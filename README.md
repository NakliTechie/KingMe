# KingMe

♟️ **Try it now → https://naklitechie.github.io/KingMe/**

Play English draughts against a minimax AI — entirely in your browser. No install, no account, no ads, nothing uploaded anywhere.

---

## What it does

- Full 8×8 English draughts against a computer opponent
- Three difficulty levels (Easy / Medium / Hard) backed by minimax search with alpha-beta pruning
- Forced-capture rule enforced — the engine only offers legal moves
- Multi-jump chains computed in full — click the destination, the piece does the rest
- King promotion with visual indicator
- Tap-to-select on mobile (no drag required)
- Last-move highlight so you always know what the AI just did
- **Correspondence mode** — every move updates the URL. Copy the link, send it to a friend, play async. No server, no login — the URL is the save file.

## How to play

1. You are **Red** (bottom). Click a piece — valid moves appear as blue dots.
2. Click a dot to move.
3. If a jump is available anywhere on the board, you must take it.
4. After a capture, keep jumping with the same piece until no further jumps are possible.
5. Reach the far end to be crowned **King** (♛) — kings move in all four diagonal directions.
6. Win by capturing all opponent pieces or leaving them with no legal moves.

## Tech

| Concern | Solution |
|---|---|
| Game logic & AI | Pure vanilla JS — minimax + alpha-beta pruning, no library |
| Board rendering | Custom SVG — no chessboard.js, no jQuery |
| Correspondence | URL hash — `btoa(JSON.stringify(state))` |
| Dependencies | **Zero** |
| Build step | **None** — open `index.html`, it works |

## Part of the NakliTechie series

| Tool | What it does |
|------|--------------|
| [**BabelLocal**](https://github.com/NakliTechie/BabelLocal) | Offline translation — 200 languages, NLLB model |
| [**StripLocal**](https://github.com/NakliTechie/StripLocal) | EXIF metadata stripper — nothing leaves the browser |
| [**GambitLocal**](https://github.com/NakliTechie/GambitLocal) | Chess vs Stockfish — correspondence mode via URL |
| [**VoiceVault**](https://github.com/NakliTechie/VoiceVault) | Audio transcription — Whisper, offline-first |
| **KingMe** | English draughts — custom minimax AI, zero deps |
| [**SnipLocal**](https://github.com/NakliTechie/SnipLocal) | Background remover — RMBG-1.4, passport mode |
| [**Clacker**](https://github.com/NakliTechie/Clacker) | Split-flap display — browser-native, offline |
| [**Strait Command**](https://github.com/NakliTechie/strait-command) | Mine-clearing game in strategic waterways |
| [**Chokepoint**](https://github.com/NakliTechie/chokepoint) | Maritime tower defense — hold the strait |
| [**PredictionMarket**](https://github.com/NakliTechie/PredictionMarket) | Prediction market simulator — Parimutuel & LMSR |
| **PDFLOcal** | PDF editor — merge, split, rotate, annotate |
| **RangeLocal** | Missile range simulator — interactive globe & map |
| [**3D Tic-Tac-Toe**](https://github.com/NakliTechie/3d-tic-tac-toe) | 3D tic-tac-toe — 3×3×3 to 5×5×5, minimax AI |

---

**Built by [Chirag Patnaik](https://github.com/NakliTechie)**
