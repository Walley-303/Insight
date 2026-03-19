# Hardware Strategy

## Overview

InSight is designed as a software-first platform built to run on smart glasses hardware. The current demos are browser-based prototypes simulating the dual-lens HUD experience.

## Dual-Lens Architecture

The core hardware assumption is two independent display surfaces:

| Lens | Role |
|------|------|
| Left | World view — document, environment, or subject being analyzed |
| Right | AI panel — intelligence, suggestions, citations, inventory data |

This separation ensures the user's physical view is never fully occluded by data overlays.

## HUD Design Principles

- **Minimal intrusion** — vignette, scanline, and corner bracket overlays stay peripheral
- **Legibility at small sizes** — UI targets clamp ranges (e.g., `clamp(8px, 1vw, 10px)`)
- **Dark-first rendering** — deep background (`#06060f`) reduces eye strain in varied lighting
- **Status indicators** — pulsing dots and live labels communicate system state at a glance

## Input Methods

- **Gaze / dwell** — primary interaction for clipping, confirming, and navigating
- **Remote control** — physical ◀ ▶ buttons for scenario navigation; clip and save actions
- **Keyboard** — arrow keys and mode shortcuts (S = Scholar, F = Field) in demo/dev mode

## Target Hardware Profile

- Lightweight smart glasses form factor
- Binocular display with independent lens rendering
- Onboard or tethered compute for AI inference
- Low-latency sensor input for gaze tracking
