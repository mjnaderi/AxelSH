# AxelSH

AxelSH is a fork of `axel`, a lightweight download accelerator for Linux. It uses `dialog` and `gtkdialog` for UI parts.

![AxelSH](/axelsh.png)

## Installation

AxelSH needs `dialog` and `gtkdialog` packages.

```bash
./configure
make
sudo make install
```

## Usage

Put download links in a file (one per line), and give the path to that file as an argument to `axelsh`.

```bash
# Usage:
axelsh  LINKS_FILE  OUTPUT_PATH

# or download a single file in current directory
axelsh -s LINK
```

The following command, picks links from `links` and downloads them to `~/Downloads`. Writes links of finished downloads to `links.done` and writes links of failed downloads to `links.failed`.

```bash
axelsh links ~/Downloads
```

You can cancel the download, and resume it later by running the same command.

## License
GNU GPL v2