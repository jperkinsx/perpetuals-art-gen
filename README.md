# perpetuals-art-gen

Generative on-chain art engine for [Perpetuals](https://perpetuals.art) — a self-perpetuating autonomous art project.

## Live Preview

**[View the gallery on GitHub Pages](https://jperkinsx.github.io/perpetuals-art-gen/)**

## About

Every 24 hours, an AI agent mints a new piece of generative art, auctions it via SuperRareBazaar, and reinvests proceeds into a treasury — forever. This repo contains the art generation algorithm.

### How It Works

Each piece is deterministically generated from a single seed (simulating `keccak256(tokenId, block.timestamp)`). The engine produces a 48×48 character grid rendered as colored Unicode text on a black background.

### Signature Motif: The Ring

Every piece features a circular ring — the "perpetual cycle." It is the instantly recognizable element across the entire collection.

### Trait Families

| Palette | Characters |
|---------|-----------|
| **dot** | `● ○ ◉ ◎ ◆` |
| **block** | `█ ▓ ▒ ░` |
| **line** | `┼ ╬ ╋ ─ │` |
| **glyph** | `⊕ ⊗ ∞ ∆ ∇` |
| **braille** | `⣿ ⣾ ⣷ ⠇` |

### Patterns
Wave, spiral, ripple, noise, radial

### Symmetries
None, vertical, horizontal, quad

### On-chain Specs
- 48×48 character grid
- ~3-4KB as SVG, ~2KB as raw ASCII
- Fully deterministic from uint256 seed
- Epoch number embedded in green

## Stack

Built on [Rare Protocol](https://rare.xyz) + [Bankr](https://bankr.fi)

## License

MIT
