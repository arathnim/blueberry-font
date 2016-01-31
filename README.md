# blueberry-font
Blueberry is a tiny, 5x10 bitmap font, made with gbdfed, designed to be clear, and as small as possible.

![scrot](https://raw.githubusercontent.com/arathnim/blueberry-font/master/font-scrot.png "blueberry")

## installation

Make a `~/.fonts` directory if you don't already have one, and `cp blueberry.bdf` into `~/.fonts`
Then, to add it to the system:

    mkfontdir ~/.fonts
    mkfontscale ~/.fonts
    xset +fp ~/.fonts/
    xset fp rehash
    fc-cache

Check `xfontsel` to make sure it's there, it'll be under the foundry `Arathnim`.

To make it so `fc-list` and `fc-match` can find your font, you'll need to do XML magic in `~/.fonts.conf`.
