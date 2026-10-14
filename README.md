# MatchPoint Live assets

Read by the MatchPoint Live app on every laptop, every 10 minutes and at start-up.

- **`sponsors/`** — every image here rotates in the sponsor-logo corner of the stream.
  Add or delete a logo on github.com (drag and drop) and every rig picks it up; nothing to
  configure on the laptop. PNG with a transparent background looks best; any aspect ratio
  is fitted into the same box.
- **`manifest.json`** — `sponsorSlideSeconds` (time per logo), `promoEveryOvers`.

Public on purpose: the app reads it without credentials. Never put stream keys or
passwords here.
