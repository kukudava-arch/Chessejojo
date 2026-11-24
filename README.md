# Stand Chess — Nebula 1.2

Mobile-first chess prototype with a Lichess/Chess.com-inspired restrained interface, trainer portrait selection, bot opponent, Stand Arrow progression, stand abilities, and spoken stand names via the device's built-in speech synthesis.

## Run locally

```bash
npm install
npm run dev
```

## Build web bundle

```bash
npm run build
```

## Android APK through GitHub Actions

1. Push this folder to a GitHub repository.
2. Open **Actions** and run **Build Android APK** (or push to `main`).
3. Download the `stand-chess-debug-apk` artifact from the completed workflow.

The workflow creates the Capacitor Android project and builds a debug APK. It is a test build, not a Play Store-signed release.

## Notes / limitations in 1.2

- Trainer portraits are original vector-style placeholders made for this prototype, not official manga panels or screenshots.
- Spoken stand names use Android/browser text-to-speech. This is real voice synthesis, but not the original Japanese/English voice actors from the anime. Availability and voice quality depend on the device's installed speech engine.
- The bot has three simple difficulty settings; it is not Stockfish and is not yet a strong chess engine.
- Online multiplayer, accounts, cloud saves, and cross-device progression are not included yet.
- Stand powers are prototype effects and are not all equivalent to the anime canon. King Crimson gives an extra move, The World delays the bot response by seven seconds, Star Platinum/Weather Report provide hints, and undo/target-scan effects are implemented for selected stands.
- The project uses the chess.js library and Capacitor Android.
