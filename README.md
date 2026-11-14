# armelstudios.github.io

Website for Armel Studios, served by GitHub Pages at https://armelstudios.github.io.

| Path | Purpose |
| --- | --- |
| `/` | Studio home page and list of games |
| `/app-ads.txt` | AdMob authorised sellers file, one for every game |
| `/lantern-grove/` | Lantern Grove page (use as the game's website if you like) |
| `/lantern-grove/privacy/` | Lantern Grove privacy policy (Google Play, AdMob consent message) |
| `/lantern-grove/privacy/#how-to-delete-your-data` | Google Play data-deletion link |

## Updating the Lantern Grove privacy policy

The policy is written once, in the game repository at `legal/PRIVACY_POLICY.md`
(the game shows the same file in Settings). After changing it there, regenerate
the page from the game repository and upload the result here:

```
python tools/export_privacy_html.py ../armelstudios.github.io
```

## Adding a game

Copy `lantern-grove/` to a new folder (for example `next-game/`), replace its
text and images, give the game its own privacy policy at `next-game/privacy/`,
and add a card for it on the home page. `app-ads.txt` already covers it.
