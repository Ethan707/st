# st - simple terminal

> st is a simple terminal emulator for X which sucks less.

**Note: This is my personal configuration of st. It is based on the original st by Aurélien APTEL.**

## Patches

- [alpha](https://st.suckless.org/patches/alpha/)
- [anysize](https://st.suckless.org/patches/anysize/)
- [colorschemes](https://st.suckless.org/patches/colorschemes/) (Partially)
- [dynamic-cursor-color](https://st.suckless.org/patches/dynamic-cursor-color/)
- [hidecursor](https://st.suckless.org/patches/hidecursor/)
- [scrollback](https://st.suckless.org/patches/scrollback/) (All patches)

Font: Meslo Nerd Font

Size: 16

Theme: One Half Dark (From the [colorschemes](https://st.suckless.org/patches/colorschemes/) patch)

## Requirements

In order to build st you need the Xlib header files.

## Installation

Edit config.mk to match your local setup (st is installed into the `/usr/local` namespace by default).

Afterwards enter the following command to build and install st (if necessary as root):

```sh
make clean install
```

## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```sh
tic -sx st.info
```

See the man page for additional details.

## Credits

Based on Aurélien APTEL <aurelien.aptel@gmail.com> bt source code.