---
title: "How to install stepmania 5 on linux 64bits"
date: 2022-01-01T14:20:27+01:00
draft: false
toc: false
images:
tags:
  - stepmania
  - linux
  - inthegroove
---
After a big long interruption here i am!

For installing it i have made an automated script

You can download at: https://nick909.nl/scripts/installstepmania.sh

Or you can install it manually:

1. Install these dependencies

>sudo apt-get install build-essential cmake mesa-common-dev libglu1-mesa-dev libglew1.5-dev libxtst-dev libxrandr-dev libpng-dev libjpeg-dev zlib1g-dev libbz2-dev libogg-dev libvorbis-dev libc6-dev yasm libasound-dev libpulse-dev binutils-dev libgtk-3-dev libmad0-dev libudev-dev libva-dev nasm

2. Clone the stepmania repo off github

>git clone --depth=1 https://github.com/stepmania/stepmania.git

3. Initialize the cloned repo s'submodules

>cd stepmania
>git submodule update --init

4. use cmake to generate a makefile

>cd Build
>cmake -G 'Unix Makefiles' -DCMAKE_BUILD_TYPE=Release .. && cmake ..

5. Build stepmania simply using the 'make' command

Note from the stepmania wiki:

>The job count passed to make should not be more than double the number of cores you have.
>e.g. -j8 if your CPU has 4 cores.

I hope this guide works!

Bye!
