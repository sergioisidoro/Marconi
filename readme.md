# Marconi is an EXPERIMENTAL ansible setup for a radio machine

Although ansible is a great tool for managing server farms, it's also
a gret tool to orchestrate local machines through playbooks, that are
Linux distro independent.

It attempts to build things from the source when possible, avoiding
adding non standard package repos, or when the non standard repos
are not availave (eg. new distos).

However we can't always do that (otherwise it would be impossible to maintain things)
Current packages that are downloaded through package repositories:

General things
* git
* make
* cmake
* build-essential
* pkg-config
* pulseaudio
* libpulse-dev

Dependencies
* gnuradio
* qt5-default
* qttools5-dev
* libqt5svg5-dev
* libsndfile1-dev
* liblapack-dev
* portaudio19-dev
* libitpp-dev

### How?

1 - Install ansible
2 - run `sudo ansible-playbook -i inventory setup-basics.yml`

### Why?
You don't need a image of an operating system. You can use your current
distro as long as it has a package repo that is supported by ansible package
instruction

## Current things installed
- gqrx
- DSD - digital speech decoder
- hackrf lib
- hamfax

## Does this work on?
- Ubuntu 18.10 yes
- ???
