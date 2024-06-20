# GameDB-GC
Nintendo GameCube (GC), part of [GameDB](https://github.com/niemasd/GameDB).

## Structured Downloads
* **[`GC.data.json`](https://github.com/niemasd/GameDB-GC/releases/latest/download/GC.data.json):** All data, structured in the JSON format
* **[`GC.data.tsv`](https://github.com/niemasd/GameDB-GC/releases/latest/download/GC.data.tsv):** All data, structured in the TSV format
* **[`GC.release_dates.pdf`](https://github.com/niemasd/GameDB-GC/releases/latest/download/GC.release_dates.pdf):** Histogram of release dates, stratified by region
* **[`GC.titles.json`](https://github.com/niemasd/GameDB-GC/releases/latest/download/GC.titles.json):** Mapping of serial numbers to game titles, structured in the JSON format

# Notes

## Uniquely Identifying Games

The game folders in [`games`](games) have the structure `DOL-XXXX-RRR`, where `XXXX` is the game code (also known as game ID), and `RRR` is the region code. The game code is at offsets `0x0000` through `0x0003` (inclusive) of the disc header, and which can be used to uniquely identify the game.

# Sources
* [Redump](http://redump.org)
