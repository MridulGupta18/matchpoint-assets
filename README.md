# MatchPoint Live assets

Read by the MatchPoint Live app on every laptop, every 4 minutes and at start-up (or instantly with the app's Sync button).

- **`sponsors/`** — every image here rotates in the sponsor-logo corner of the stream.
  Add or delete a logo on github.com (drag and drop) and every rig picks it up; nothing to
  configure on the laptop. PNG with a transparent background looks best; any aspect ratio
  is fitted into the same box.
- **`ads/`** — the video ads (MP4, MOV, MKV or WebM; any resolution, fitted to 1080p). Each
  file becomes a button in the app's Video ads panel ("willow-sports.mp4" -> "Willow Sports"),
  the "All in series" button plays them in name order, and the every-N-overs auto-promo
  rotates through them. Keep each under ~50 MB (GitHub's web upload limit is 25 MB per file;
  use `git push` for bigger ones, hard limit 100 MB).
- **`manifest.json`** — `sponsorSlideSeconds` (time per logo), `promoEveryOvers`.

Public on purpose: the app reads it without credentials. Never put stream keys or
passwords here.
