# asdf-R

[R](https://www.r-project.org/) plugin for [asdf](https://github.com/asdf-vm/asdf) version manager.

## Dependencies

* Mac
    1. [Homebrew](https://brew.sh): used to install the remainder of the dependencies
    1. ```brew install --cask xquartz```
    1. ```brew install gcc xz bzip2 pcre2```
    1. See the note below
* Linux
    * Ubuntu / Debian
        1. ```sudo apt-get install build-essential libcurl3-dev libreadline-dev gfortran libbz2-dev liblzma-dev libpcre3 libpcre3-dev```

### Mac Notes

After installing the other dependencies, you may need to modify your environment a bit in order to pick
up the dependencies from homebrew.

```
# Set bzip2 binary and compile paths
export PATH="/usr/local/opt/bzip2/bin:$PATH"
export CPPFLAGS="-I/usr/local/opt/bzip2/include $CPPFLAGS"
export LDFLAGS="-L/usr/local/opt/bzip2/lib $LDFLAGS"

# Set pcre2 binary and compile paths
export PATH="/usr/local/opt/pcre2/bin:$PATH"
export CPPFLAGS="-I/usr/local/opt/pcre2/include $CPPFLAGS"
export LDFLAGS="-L/usr/local/opt/pcre2/lib $LDFLAGS"
```

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
