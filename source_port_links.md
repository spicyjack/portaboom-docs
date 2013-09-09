# List of Doom Source Ports and Dependencies #

## Doom Source Ports ##

### Chocolate Doom ###
- Homepage: http://www.chocolate-doom.org/wiki/index.php/Chocolate_Doom
- Downloads: http://sourceforge.net/projects/chocolate-doom/files/
- Command line arguments:
  http://www.chocolate-doom.org/wiki/index.php/Command_line_arguments
- License: GPLv2 or later
- Renderer: software
- SDL requirements: mixer, net

### Doom Legacy ###
- Homepage: 
- Wiki: http://legacywiki.net/index.php/Main_Page (SVN downloads, lower right
  hand corner)
- Downloads: http://doomlegacy.sourceforge.net/
- Command line arguments: http://tinyurl.com/nez6q4 (SVN repo;
  doomlegacy/legacy/trunk/docs/legacy.html)
- License: GPLv2 or later
- Renderer: software, OpenGL
- SDL requirements: mixer, video

### DoomsdayEngine ###
- Homepage: http://dengine.net/
- Downloads: http://sourceforge.net/projects/deng/files/
- How to compile page:
  http://www.dengine.net/dew/index.php?title=How_to_compile
- Running Doomsday:
  http://www.dengine.net/dew/index.php?title=Running_Doomsday_in_Unix
- Command line arguments:
  http://www.dengine.net/dew/index.php?title=Command_line_options_reference
- License: GPLv2 or later
- Renderer: software?, OpenGL?
- SDL requirements: mixer, net  

### EDGE (Enhanced Doom Game Engine) ###
- Homepage: http://edge.sourceforge.net/
- Downloads: http://sourceforge.net/projects/edge/files/EDGE%20Source%20Code/
- Command line arguments: http://tinyurl.com/lrhguc (SVN HEAD)
- License: GPLv2 or later
- Renderer: software?, OpenGL?
- SDL requirements: image, mixer, net  

### Eternity Engine ###
- Homepage: http://eternity.youfailit.net/index.php?title=Eternity_Engine
- Downloads:
  http://www.doomworld.com/vb/eternity/49268-eternity-engine-3-37-00-sekhmet/
- Command line arguments:
  http://eternity.youfailit.net/index.php?title=List_of_command_line_parameters
- License: GPLv2
- Renderer: software?, OpenGL?
- SDL requirements: mixer, net, video

### GZDoom ###
- Homepage: http://www.osnanet.de/c.oelckers/gzdoom/index.html
- SVN Repo: http://mancubus.net/svn/gzdoom 
  - check out code with `svn checkout
    http://mancubus.net/svn/hosted/gzdoom/tags/1.5.06 gzdoom-1.5.06`
- Command line arguments: http://zdoom.org/wiki/Command_line_parameters
- Compiling: http://zdoom.org/wiki/Compile_ZDoom_on_Linux
- License: [idSoftwareDoomLicense]
- Renderer: OpenGL
- SDL requirements: video

### Odamex ###
- Homepage: http://odamex.net/
- Downloads: http://sourceforge.net/projects/odamex/files/
- Command line arguments: Source code
- License: GPLv2 or later
- Renderer: software?, OpenGL?
- SDL requirements: mixer, video

### PrBoom ###
- Homepage: http://prboom.sourceforge.net/linux.html
- Downloads: http://sourceforge.net/projects/prboom/files/
- Command line arguments: http://tinyurl.com/mqyeza (SVN HEAD)
- License: GPLv2 or later
- Renderer: software, OpenGL
- SDL requirements: mixer, net

### PrBoom+ ###
- Homepage: http://prboom-plus.sourceforge.net/
- Downloads: http://sourceforge.net/projects/prboom-plus/files/
- Command line arguments: http://tinyurl.com/mqyeza
- License: GPLv2 or later
- Renderer: software, OpenGL
- SDL requirements: mixer, net

### ReMooD ###
- Homepage: http://remood.org/
- Downloads: http://remood.org/?page=download
- Command line arguments: http://tinyurl.com/nrapnf (SVN HEAD)
- License: GPLv3 or later (in repo, 08a is still GPL2)
- Renderer: software?, OpenGL?
- SDL requirements: ?

### Vavoom ###
- Homepage: http://vavoom-engine.com/
- Downloads: http://vavoom-engine.com/download.php
- Command line arguments:
  http://vavoom-engine.com/wiki/index.php?title=Command_line_arguments
- License: GPLv2 or later
- Renderer: software?, OpenGL?
- SDL requirements: mixer, video

### ZDoom ###
- Homepage: http://zdoom.org/News
- Downloads: http://zdoom.org/Download
- Command line arguments: http://zdoom.org/wiki/Command_line_parameters
- Compiling: http://zdoom.org/wiki/Compile_ZDoom_on_Linux
- License: [idSoftwareDoomLicense]
- Renderer: software
- SDL requirements: video

## Quake Source Ports ##

### Darkplaces ###
- Homepage:
- License: GPLv2 or later
- Renderer: ?
- SDL requirements: video

### EZQuake ###
- Homepage:
- Renderer: ?
- License: GPLv2 or later

### Fitzquake ###
- Homepage:
- Renderer: ?
- License: GPLv2 or later
- Doesn't build

### FODQuake ###
- Homepage:
- License: GPLv2 or later
- Renderer: ?

### FTEQuake ###
- Homepage:
- License: GPLv2 or later
- Renderer: ?
- SDL requirements: video

### JoeQuake ###
- Homepage:
- License: GPLv2 or later
- Renderer: ?
- SDL requirements: video
- Doesn't build

### Quakeforge ###
- Homepage:
- License: GPLv2 or later
- Renderer: ?
- SDL requirements: video

### Quakespasm ###
- Homepage:
- License: GPLv2 or later
- Renderer: ?
- SDL requirements: net

### Quore ###
- Homepage:
- License: GPLv2 or later
- Renderer: ?

### TyrQuake ###
- Homepage:
- License: GPLv2 or later
- Renderer: ?

## Library Dependencies ##

### libSDL (base, mixer, net, image, ttf) ###
- License: LGPL2 or later

### alsa-lib ##
- License: ?

### dbus ###
- License: ?

### expat ###
- License: ?

### flac ###
- License: ?

### fluidsynth ###
- License: ?

### libffi ###
- License: ?

### libmikmod ###
- License: ?

### libogg ###
- License: ?

### libsndfile ###
- License: ?

### libvorbis ###
- License: ?

### smpeg ###
- License: ?

### util-linux ###
- License: ?

### libglib ###
- License: ?

### pkg-config ###
- License: ?

# Misc #

## Generating lists of files that use SDL ## Generate a list of files that
refer to SDL with:

    cd ~jenkins/jobs find . -mindepth 3 -maxdepth 3 -type d | grep workspace \
    | grep -v lib | egrep -v "artifacts|output|temp" | sort \ | xargs grep
    -rns "SDL" 


vim: set filetype=markdown shiftwidth=2 tabstop=2 
