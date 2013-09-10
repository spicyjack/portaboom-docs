# List of Portaboom Library Dependencies #

## libSDL (base, mixer, net, image, ttf) ##
- Homepage: http://www.libsdl.org/
- Downloads: http://www.libsdl.org/download-1.2.php
- License: LGPL2.1 or later
- Builds with: GNU `make`

## alsa-lib ##
- Homepage: http://www.alsa-project.org/main/index.php/Main_Page
- Downloads: ftp://ftp.alsa-project.org/pub/lib/
- License: LGPL2.1 or later
- Builds with: GNU `make`

## dbus ##
- Homepage: http://www.freedesktop.org/wiki/Software/dbus/
- Downloads: http://dbus.freedesktop.org/releases/dbus/
- License: Academic License 2.1 **or** GPL2 or later
- Builds with: GNU `make`

## expat ##
- Homepage:
- Downloads:
- License: Expat license (X11-ish)
- Builds with:

## flac ##
- Homepage:
- Downloads:
- License: libFLAC: 3-clause BSD., flac: GPL2 or later
- Builds with:

## fluidsynth ##
- Homepage:
- Downloads:
- License: LGPL2 or later
- Builds with:

## libffi ##
- Homepage:
- Downloads:
- License: X11
- Builds with:

## libmikmod ##
- Homepage:
- Downloads:
- License: LGPL2 or later
- Builds with:

## libogg ##
- Homepage:
- Downloads:
- License: ?
- Builds with:

## libsndfile ##
- Homepage:
- Downloads:
- License: ?
- Builds with:

## libvorbis ##
- Homepage:
- Downloads:
- License: ?
- Builds with:

## smpeg ##
- Homepage:
- Downloads:
- License: ?
- Builds with:

## util-linux ##
- Homepage:
- Downloads:
- License: ?
- Builds with:

## libglib ##
- Homepage:
- Downloads:
- License: ?
- Builds with:

## pkg-config ##
- Homepage:
- Downloads:
- License: ?
- Builds with:

# Misc #

## Generating lists of files that use SDL ## Generate a list of files that
refer to SDL with:

    cd ~jenkins/jobs find . -mindepth 3 -maxdepth 3 -type d | grep workspace \
    | grep -v lib | egrep -v "artifacts|output|temp" | sort \ | xargs grep
    -rns "SDL" 


vim: set filetype=markdown shiftwidth=2 tabstop=2 
