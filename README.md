# GameDB-GC
Nintendo GameCube (GC), part of [GameDB](https://github.com/niemasd/GameDB).

## Structured Downloads
* **[`GC.data.json`](https://github.com/niemasd/GameDB-GC/releases/latest/download/GC.data.json):** All data, structured in the JSON format
* **[`GC.data.tsv`](https://github.com/niemasd/GameDB-GC/releases/latest/download/GC.data.tsv):** All data, structured in the TSV format
* **[`GC.release_dates.pdf`](https://github.com/niemasd/GameDB-GC/releases/latest/download/GC.release_dates.pdf):** Histogram of release dates, stratified by region
* **[`GC.titles.json`](https://github.com/niemasd/GameDB-GC/releases/latest/download/GC.titles.json):** Mapping of serial numbers to game titles, structured in the JSON format

# Notes

## Uniquely Identifying Games

The game folders in [`games`](games) have the structure `DOL-XXXX-RRR`, where `XXXX` is the game code (also known as game ID), and `RRR` is the region code. The game code is stored directly within the disc and can be used to uniquely identify the game. I currently use the [`gciso` Python package](https://gciso.readthedocs.io/en/latest/#gciso.IsoFile.gameCode) to extract the game code (and other metadata) from a GameCube disc image. See the [GameID GameCube identification code](https://github.com/niemasd/GameID/blob/9cbbcf62b0123ede7ff6e835a0c7374f6d2ad6b8/GameID.py#L302-L340) for implementation details.

# Sources
* [Redump](http://redump.org)
