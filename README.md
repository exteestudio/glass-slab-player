# Glass Slab Player

A music player prototype built around a slab of liquid glass: a spinning disc, a refracting glass panel,
synced lyrics on a card that slides out from behind the player, and macOS window controls.
One HTML file, no build step, no dependencies.

**[Play the live demo →](https://exteestudio.github.io/glass-slab-player/)**

## What's in it

- A liquid-glass slab that bends the spinning disc beneath it, with frosting and a red/green/blue split
  at the edges (SVG displacement filters).
- A disc that spins up on play, coasts to a stop on pause, and flies out and back in with motion blur when
  you skip.
- Time-synced lyrics on a second card that slides out from behind the player. Tap a line to jump there.
- Long titles stay on one line and scroll with soft edge fades.
- A scrub bar that lifts on hover, with a floating time pill.
- A five-song shuffle playlist that loops.

## Run it

Open `index.html` in Safari or Chrome. Everything is inside that one file, apart from two things it loads
while you're online:

- **Album covers** from Apple's iTunes catalogue (iTunes Search API). Offline, the discs show a plain
  placeholder.
- **Synced lyrics** from [LRCLIB](https://lrclib.net). Offline, the lyrics card stays empty.

There's no audio: the playhead is simulated.

## Fonts

The design uses Neue Montreal by Pangram Pangram, a commercial font that isn't included here. If you have
it installed, Chrome uses it. Safari never lets web pages use installed fonts, so Safari, and anyone
without the font, sees Hanken Grotesk instead, which is embedded under the SIL Open Font License
(see `OFL.txt`).

To use Neue Montreal everywhere, get a web license from Pangram Pangram and replace the `local(...)`
sources in the `@font-face` rules at the top of `index.html` with your licensed font files.

## Credits

- Album artwork belongs to its rights holders and is loaded from Apple at runtime. Lyrics are loaded from
  LRCLIB at runtime. Song and artist names are only used to identify the music.
- This is an independent design prototype. It isn't affiliated with or endorsed by Drake, Apple or LRCLIB.
- Hanken Grotesk © The Hanken Grotesk Project Authors, SIL Open Font License 1.1.

## License

The code and original design assets are MIT licensed (see `LICENSE`). That license doesn't cover the
third-party content the page loads at runtime (album artwork, lyrics) or the fonts named above.
