# WotLK World Maps

World map textures from World of Warcraft: Wrath of the Lich King (3.3.5a),
in 5 locales (deDE, enGB, esES, frFR, ruRU), plus `ZoneIDs.json` mapping each
map file name to its in-game zone ID and full zone name.

## Contents
- `<locale>/*.png` - 79 world map textures per locale (1002×668 px)
- `ZoneIDs.json` - array of `{ filename, id, name }` (74 zones)

`filename` matches the PNG file name without extension (e.g. `Durotar` ->
`<locale>/Durotar.png`).

```json
[
  { "filename": "Durotar", "id": 14, "name": "Durotar" },
  { "filename": "Alterac", "id": 36, "name": "Alterac Mountains" }
]
```

> Note: there are 79 images but 74 entries in `ZoneIDs.json`. The 5 extra
> images are continent / world maps (`Azeroth`, `Kalimdor`, `Northrend`,
> `Cosmic`, `World`), which are not zones and have no zone ID.

## Disclaimer
All map textures, as well as every value in `ZoneIDs.json` — the map/zone names
(`filename`), the full zone names (`name`), and the zone IDs (`id`) — are
© Blizzard Entertainment, Inc. and are taken from / derived from World of
Warcraft game data. World of Warcraft and Warcraft are trademarks of Blizzard
Entertainment. This is an unofficial, non-commercial fan project and is not
affiliated with or endorsed by Blizzard.

The MIT License (see [`LICENSE`](LICENSE)) applies ONLY to this repository's own
documentation and to the format/structure (the schema) of `ZoneIDs.json` — NOT
to the Blizzard-owned image assets or to any of the values contained in
`ZoneIDs.json` (`filename`, `name`, `id`). See the `LICENSE` file for the full
scope and the third-party notice.
