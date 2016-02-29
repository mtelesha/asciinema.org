<% content_for(:title, 'Installation') %>

# Installation

## Using package manager

### OS X

Homebrew:

<%= render 'install_homebrew' %>

MacPorts:

    sudo port selfupdate && sudo port install asciinema

Nix:

    nix-env -i go1.4-asciinema

### Arch Linux

    yaourt -S asciinema

### Debian

    sudo apt-get install asciinema

### Fedora

    sudo yum install asciinema

### FreeBSD

Ports:

    cd /usr/ports/textproc/asciinema && make install

Packages:

    pkg install asciinema

### Gentoo Linux

    layman -a go-overlay && emerge -av asciinema

### NixOS / Nix

    nix-env -i go1.4-asciinema

### Ubuntu

    sudo apt-add-repository ppa:zanchey/asciinema
    sudo apt-get update
    sudo apt-get install asciinema

### OpenSUSE

Leap 4.1

    #  OCICLI https://software.opensuse.org/ymp/network/openSUSE_Leap_42.1/asciinema.ymp?base=openSUSE%3ALeap%3A42.1&query=asciinema
OpenSUSE 13.2

    # OCICLI https://software.opensuse.org/ymp/network/openSUSE_13.2/asciinema.ymp?base=openSUSE%3A13.2&query=asciinema
    
One Click Install for all supported versions

    https://software.opensuse.org/package/asciinema?search_term=asciinema

### No package for your operating system?

If you use other operating system and you can build a native package
for it then don't hesitate, do it and let us know.

## From source

If you have Go toolchain installed you can install latest (master) version with:

    go get github.com/asciinema/asciinema

Refer to the
[README file](https://github.com/asciinema/asciinema/blob/master/README.md)
for detailed instructions on building from source.

## Download static binary

There are prebuilt static binaries for Mac OS X, Linux and FreeBSD. You can
[download](https://github.com/asciinema/asciinema/releases) one for your
platform and place it in your `$PATH`.

You can use the following snippet to fetch and run our install script, which automates this:

    curl -sL https://asciinema.org/install | sh
