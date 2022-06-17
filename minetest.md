# Getting Minetest
First off, you will need Minetest.

## Windows
https://www.minetest.net/downloads/

## Linux
Linux has the terminal install methods, but it is best if you have a a minimum Minetest version of 5.4.0. Minetest's README file will work in helping you build your own version, but if that doesnt work then do the following:

For Debian/Ubuntu users:

    sudo apt install g++ make libc6-dev cmake libpng-dev libjpeg-dev libxxf86vm-dev libgl1-mesa-dev libsqlite3-dev libogg-dev libvorbis-dev libopenal-dev libcurl4-gnutls-dev libfreetype6-dev zlib1g-dev libgmp-dev libjsoncpp-dev libzstd-dev libluajit-5.1-dev

For Fedora users:

    sudo dnf install make automake gcc gcc-c++ kernel-devel cmake libcurl-devel openal-soft-devel libvorbis-devel libXxf86vm-devel libogg-devel freetype-devel mesa-libGL-devel zlib-devel jsoncpp-devel gmp-devel sqlite-devel luajit-devel leveldb-devel ncurses-devel spatialindex-devel libzstd-devel

For Arch users:

    sudo pacman -S base-devel libcurl-gnutls cmake libxxf86vm libpng sqlite libogg libvorbis openal freetype2 jsoncpp gmp luajit leveldb ncurses zstd

For Alpine users:

    sudo apk add build-base cmake libpng-dev jpeg-dev libxxf86vm-dev mesa-dev sqlite-dev libogg-dev libvorbis-dev openal-soft-dev curl-dev freetype-dev zlib-dev gmp-dev jsoncpp-dev luajit-dev zstd-dev
    
After you install dependancies, you can install the source code:

    git clone https://github.com/minetest/minetest.git
    cd minetest
   
Checkout Minetest Version 5.5.1

    git checkout 5.5.1
        
Download IrrlichtMt to `lib/irrlichtmt`, it will be used to satisfy the IrrlichtMt dependency that way:

    git clone --branch 1.9.0mt5 https://github.com/minetest/irrlicht.git lib/irrlichtmt
    
Build a version that runs directly from the source directory:

    cmake . -DRUN_IN_PLACE=TRUE
    make -j$(nproc)
    
And install it on your system:

    make install
    
    
If you run Ubuntu, another way to get minetest is:

    sudo add-apt-repository ppa:minetestdevs/stable
    sudo apt update
    sudo apt install minetest
    
## Mac
Follow instructions [here](https://www.minetest.net/downloads/)

## Notes
All instructions available at https://github.com/minetest/minetest/blob/master/README.md .
