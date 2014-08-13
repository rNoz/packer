# README


## Introduction

Modification of [keenerd/packer](https://github.com/keenerd/packer) to allow using *BitBucket* [AUR](https://aur.archlinux.org)-like repo and `--force` arg for 
`pacman`.

## Use

Because I currently use `packer` (although I still keep `yaourt`) I have modified
the original repo to be able to use a specific git repository from *BitBucket*. 
It should be easy to adapt it for the *Github* API.

Currently it is only supported the install function:
`packer --bbrepo g4lbb:aur -S package-name`

Another feature added to this modification is the possibility to `force` the installation.
It is something that I missed from the original `packer`:

-   `packer --force -S package-name`, or
-   `packer --bbrepo g4lbb:aur --force -S package-name`

I have used the repo [g4lbb AUR](https://bitbucket.org/g4lbb/aur). With this system it is possible to create alternative
AUR distributed repos (public or private). So far it is not as comfortable as the real AUR,
but it is possible to use this alternative.

## TODO 

-   github AUR-like support (`--ghrepo` or similar)
-   allow searches
-   allow updates

They are **not planned** for the near future because these modifications solves
my problems/requests. If you want to modify again or allow more options, do it or request to me ;)

## Authors

Original project:

-   Matthew Bruening <matthewbruenig@gmail.com>

Modification:

-   Raúl Nozal <rnoz.commits@gmail.com>

## License

GNU GPLv3