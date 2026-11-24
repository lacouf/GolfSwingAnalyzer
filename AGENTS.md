# Agent instructions

## Project goal

Build a macOS app that helps a golfer review practice sessions recorded from two iPhones: one down-the-line view and one face-on view. The first useful version imports two recordings, synchronizes them, finds or lets the user mark swings, and compares clips with a 2D body-joint overlay.

## Product and engineering constraints

- Target macOS first; use Swift and SwiftUI unless a documented decision changes this.
- Keep video processing on the Mac for the first version. Do not add a server, account system, or cloud upload.
- Treat pose landmarks as estimates. Display confidence and avoid presenting them as medical or coaching diagnoses.
- Start with 2D pose overlays per camera. Do not build 3D reconstruction or automated swing coaching in the MVP.
- Preserve source videos and their frame timing. Do not assume slow-motion playback timestamps equal capture time.
- Prefer small, reviewable changes and explain tradeoffs in plain language.
- Do not add dependencies without explaining why they are needed.
- Do not add or run tests unless the user asks for tests or verification.

## Working with the user

- The user is a software developer but new to Apple development. Explain Xcode and macOS-specific steps clearly.
- Ask before actions that publish externally or incur costs. Never commit secrets, personal videos, or generated media.
- Keep product decisions in `docs/DECISIONS.md` and the current scope in `docs/PRODUCT.md`.

## Before changing code

Read this file and `README.md`. If you change the architecture or MVP scope, update the relevant docs in the same change.
