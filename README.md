# TT Data Chunks

Transit time and distance data for the TT Fetcher userscript.

## Structure

- `manifest.json` — Lists all chunk files and the data version
- `tt-data-part1.json` to `tt-data-part11.json` — Route data split into chunks under 10 MB each

## Format

Each chunk is a JSON object where:
- **Key**: `ORIGIN->DESTINATION` (e.g. `BCN8->DCT9`)
- **Value**: `| Route:ORIGIN->DESTINATION, Distance = X (Km) , Transit Time = Y (hours) .`

## Stats

- Total routes: 1,001,322
- Version: 2026-07-27
- Chunks: 11 (~9 MB each)

## Usage

This data is auto-synced by the TT Fetcher userscript via the manifest file. No manual download needed.
