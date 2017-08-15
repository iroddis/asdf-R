# asdf-r

[R](https://www.r-project.org/) plugin for [asdf](https://github.com/asdf-vm/asdf) version manager

## Dependencies

1. You will need a compiler.
  * Mac
    1. ```gcc```
    1. Hit the ok button and it will install.  If it already has it, then you are good.
  * Ubuntu
    1. ```sudo apt-get install linux-headers-$(uname -r) build-essential```
1. On Ubuntu, you will need libreadline and libcurl
  1. ```sudo apt-get install libreadline-dev libcurl3-dev```

## Install

```
asdf plugin-add postgres https://github.com/iroddis/asdf-r.git
```

## ASDF options

Check [asdf](https://github.com/asdf-vm/asdf) readme for instructions on how to install & manage versions of R.

When installing R using `asdf install`, you can pass custom configure options with the following env vars:

* `R_CONFIGURE_OPTIONS` - use only your configure options
* `R_EXTRA_CONFIGURE_OPTIONS` - append these configure options along with ones that this plugin already uses

## Thanks

Thanks to (asdf-postgres)[http://github.com/smashedtoatoms/asdf-postgres] for providing an awesome plugin
that was easy to modify for this language.
