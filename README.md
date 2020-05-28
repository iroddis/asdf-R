# asdf-R

[R](https://www.r-project.org/) plugin for [asdf](https://github.com/asdf-vm/asdf) version manager.

## Dependencies

* Mac
    1. [Homebrew](https://brew.sh): used to install the remainder of the dependencies
    1. ```brew install gcc xz```
* Linux
    * Ubuntu / Debian
        1. ```sudo apt-get install build-essential libcurl3-dev libreadline-dev gfortran xorg-dev libbz2-dev liblzma-dev libpcre2-dev```

## Install

```
asdf plugin-add R https://github.com/iroddis/asdf-R.git
```

## ASDF options

Check [asdf](https://github.com/asdf-vm/asdf) readme for instructions on how to install & manage versions of R.

When installing R using `asdf install`, you can pass custom configure options with the following env vars:

* `R_CONFIGURE_OPTIONS` - use only your configure options
* `R_EXTRA_CONFIGURE_OPTIONS` - append these configure options along with ones that this plugin already uses

## Thanks

Thanks to [asdf-postgres](http://github.com/smashedtoatoms/asdf-postgres) for providing an awesome plugin
that was easy to modify for this language.
