# Deploy Masters TCG 🕹️

A retro 8-bit trading card game where the cards are the team. Two players battle
on one keyboard — or against a CPU opponent — until someone's HP hits zero.

Built with plain HTML + CSS + JS. No backend, no dependencies, no install:
everything runs in the browser.

## Play

Open `index.html` in any browser, or play the hosted version:

> https://wandacrohare.github.io/darcy-test-dispatch/

## How to play

- **Energy** refills every turn: turn 1 gives you 1, turn 2 gives 2, and so on
  up to 10. Unspent energy is lost. Playing a card and attacking both spend from
  the same pool.
- **Play cards** by paying their yellow cost. The first one becomes your
  **active**; the rest go to the **bench** (3 spots).
- **Attack** with your active as many times as your energy allows. Damage hits
  the enemy active — if they have no active, it hits **them directly**.
- Each player has **30 HP**. Bring the other player's HP to 0 to win.
- Once per turn you can **switch** your active with a benched card, for free.
- A card can attack on the same turn it's played.
- Player 2 can be a **human** or a **CPU** — toggle it on the start screen.

## The roster

| Card | Role | ★ | HP | Cost |
|---|---|---|---|---|
| **James** — The Architect | Structural damage and defense | ★★ | 90 | 3 |
| **Travis** — The Project Owner | Re-prioritizes your life | ★★ | 80 | 4 |
| **DARCYIQ** — The Legendary AI | Absurdly OP holo card | ★★★ | 150 | 5 |
| **Nico** — Programmer | Ships bugs as features | ★ | 55 | 2 |
| **Christian** — Programmer | Code review as a weapon | ★ | 45 | 1 |
| **Fernando** — Programmer | Force pushes to main | ★ | 60 | 2 |
| **Alexis** — Programmer | Refactors at 3 AM | ★ | 50 | 2 |
| **Enzo** — Programmer | Copy-paste artisan | ★ | 50 | 2 |
| **Wanda** — The UX | Redesigns your board | ★ | 45 | 1 |

A legendary DARCYIQ card hides in one of the decks each match (coin flip per
deck). If it reaches the board, you'll know.

## Features

- **4 switchable themes**: retro 8-bit, neon cyberpunk, pastel kawaii and epic fantasy (palette, typography and borders change; preference is saved)
- Theme-matched avatars: procedural pixel sprites in retro, emoji on color orbs in neon/kawaii (🎨 Wanda, 🤖 DarcyIQ, 🏗️ James…), and golden letter-sigil medallions in fantasy
- Mana-style energy, bench switching, direct hits, overflow damage, KO promotions
- Optional CPU opponent with deploy/attack/retreat heuristics
- **English and Spanish** — toggle the language button anytime, even mid-match
- Retro WebAudio bleeps (mutable), attack animations, screen shake
- Mobile responsive
- Everything in a single self-contained `index.html`

## Development

```
open index.html
```

That's the whole toolchain. Edit the `CHARS` array to add or rebalance cards.
