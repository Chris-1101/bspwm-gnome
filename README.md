# bspwm-gnome [![Maintenance](https://img.shields.io/maintenance/no/2020.svg)]()
### An [i3-gnome](https://github.com/i3-gnome/i3-gnome) fork for bspwm

Allows you to use bspwm with GNOME 3 Session infrastructure.


## Requirements
* bspwm
* GNOME (3.36.x)
* GDM (optional, but useful)
* [GNOME Flashback](https://github.com/i3-gnome/i3-gnome/wiki/Tips-&-Tricks#gnome-flashback) (Optional)

## Installation (`make`)
Using `make`:
* `git clone git@github.com:Chris-1101/bspwm-gnome.git`.
* `cd bspwm-gnome`
* `sudo make install`

## Installation (`aurutils`)
If you're on Arch Linux and using `aurutils`, you can use the `PKBUILD` file to build `bspwm-gnome` to your local pacman repo. It's a bit of a manual fiddle as I haven't bothered properly submitting this to the AUR, but it gets the job done avoiding foreign packages:
* `git clone git@github.com:Chris-1101/bspwm-gnome.git`
* `cd bspwm-gnome/makepkg`
* `makepkg -s`
* `mv bspwm-gnome-*.pkg.tar.zst /var/cache/pacman/REPO_NAME/`
* `repo-add n /var/cache/pacman/REPO_NAME/REPO_NAME.db.tar /var/cache/pacman/REPO_NAME/bspwm-gnome-VERSION.pkg.tar.zst`
* `sudo pacman -Syu`
* `sudo pacman -S bspwm-gnome`

