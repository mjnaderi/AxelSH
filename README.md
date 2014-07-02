# AxelSH

My simple download manager for linux!

Uses `axel` for downloading and accelerating downloads. Uses `zenity` and `gtkdialog` for GUI dialogs.

## Requirements

AxelSH needs `zenity` and `gtkdialog` packages.

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
axelsh LINKS_FILE FINISHED_LINKS_FILE OUTPUT_PATH
```

The following command, picks a link from `links` and downloads it to `~/Downloads`, and moves that link from `links` to `finished_links`, and repeats this for all links in `links`.

```bash
./axelsh links finished_links ~/Downloads
```

You can cancel the download and resume it later by running the same command.

## License
GNU GPL v3