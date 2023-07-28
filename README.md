# Lines Are Rusty

Re-implementation of https://github.com/ax3l/lines-are-beautiful in Rust.

Very, very early version.
Just for the fun of it, with great contributions from Tim Ryan @tcr .

File format:
https://plasma.ninja/blog/devices/remarkable/binary/format/2017/12/26/reMarkable-lines-file-format.html


## Install via Cargo
Install rustup: https://rustup.rs/

```bash
cargo install --git https://github.com/ax3l/lines-are-rusty.git --branch develop

# Binary should now be available on your path
lines-are-rusty --help
```

## Usage

```bash
# Render SVG from notebook page
lines-are-rusty notebook-page.rm -o notebook-page.svg

# Render PDF from notebook page
lines-are-rusty notebook-page.rm -o notebook-page.pdf
```

## Changelog

### 2023-08
* implemented support for colors of the highlighter brush
* extended the custom-colors -> you now need to specify 9 colors per layer if you want to overwrite them
* using grey as fallback for unexpected colors
* got rid of a couple build warnings
