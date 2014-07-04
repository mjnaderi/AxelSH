# AxelSH

My simple download manager for linux!

Uses `axel` for downloading and accelerating downloads. Uses `dialog` and `gtkdialog`.

## Requirements

AxelSH needs `dialog` and `gtkdialog` packages.

Before start, you need to compile my modified version of `axel`:

```bash
cd axel
./configure
make
```

## Usage

Put download links in a file (one per line), and give the path to that file as an argument to `axelsh`.

```bash
# Usage:
axelsh  LINKS_FILE  OUTPUT_PATH
```

The following command, picks links from `links` and downloads them to `~/Downloads`. Writes links of finished downloads to `links.done` and writes links of failed downloads to `links.failed`.

```bash
./axelsh links ~/Downloads
```

You can cancel the download, and resume it later by running the same command.

## License
GNU GPL v3