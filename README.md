# Hologram Viewer

A free web page that turns any tablet or phone into a Pepper's ghost hologram display. Play the built-in high-resolution hologram videos, or show your own videos, images and 3D models, mirrored on a black background.

Made for the *Tabletop Hologram Stand* on MakerWorld, but it works with any sheet of clear acrylic at 45°.

## Features

- **Video library:** 1080p loops rendered for hologram use: pure black background, bright subject, seamless loop
- **Your own files:** pick several at once to make a playlist. Video (mp4/mov), image (png/jpg/gif) or 3D model (.glb, in its real colours or as a wireframe)
- **Mirror** (up–down, sideways, off) and **rotate**, so the reflection reads correctly
- Size, brightness and "darken background" for videos that don't have a fully black background
- Extras: a clock and your own text
- The controls hide on their own. Tap to bring them back.
- Settings and the last video are remembered. Your files never leave your device.
- Runs on old devices too (down to iOS 12 / iPad Air 1)

## Use it

Open the page on your tablet. On iPhone or iPad, choose Share → Add to Home Screen and open it from there to get full screen.

## Add your own videos to the library

Put the mp4 and a small poster jpg in `videos/` and add a line to `videos/videos.json`:

```json
{"file": "videos/my-clip.mp4", "title": "My clip", "poster": "videos/my-clip.jpg"}
```

For the best hologram, use a pure black background. H.264 1080p at up to level 4.0 plays on old iPads.

## Host it yourself

It's a static site. Put `index.html`, `lib/` and `videos/` on any web host, for example GitHub Pages or Netlify.

## Licence

Code: MIT. three.js © three.js authors (MIT). Videos: CC BY 4.0.
