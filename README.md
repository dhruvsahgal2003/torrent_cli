
## Features

- Search torrents from multiple indexers
- Fetch magnet links directly
- Download torrents via libtorrent
- Pretty CLI with Rich-powered progress bars
- Modular and easily extensible indexer architecture

## Installation

Requirements: Python 3.13+ and [libtorrent](https://libtorrent.org/).

```bash
pipx install torrra
```

> Works on all platforms using the pip-installed libtorrent.

For local development:

```bash
git clone https://github.com/dhruvsahgal2003/torrent_cli
cd torrra
# or use requirements.txt
uv sync
uv run torrra
```

## Indexer Support

Currently supported:

- YTS (movies)
- MagnetDL
- Movierulz (moviesr)

## Dev Notes

- Modular indexer structure (`torrra/indexers`)
- Extend `BaseIndexer` to add new sources
- Built using:
  - `httpx` + `selectolax` for scraping
  - `libtorrent` for torrenting
  - `rich` for CLI visuals
  - `questionary` for input prompts

