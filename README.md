Bochs [![Build Status](https://travis-ci.org/benjojo/bochs.png?branch=master)](https://travis-ci.org/benjojo/bochs)
=====



My version of bochs that has a silly visualisation of RAM.

## To use
This version of Bochs has been modified so that every time a ram *write* happens a log of the event is taken down.

This event is stored in `ram.dat` with each event costing you about 16 bytes of disk space, In my testing I've never seen logging go over 1MB/s but this is because I've been testing with a broken livecd! So if you load windows or something else in I can't say how fast you will be logging (hopefully not too much though)

I've only tested this on Debian 7 so I am unable to say if the changes I have made work in Window and OSX.

Once you are in. Go into the `bochs` folder and run `./configure` wait for it to generate a make file for you.

Then `make all` and wait a bit for it to build. After that is done you will have the first step in the tools I have built.

Go and setup a bochsrc and then run your VM, after you have concluded you have collected enough data. Exit out of bochs and then make your way to the `bochs_vizzi` folder and compile that using `mono`.

Once you have that. Feed it the `ram.dat` that bochs produced and go and do something else for a while since its going to take a while to make all the frames needed.

## Demo
Coming *soon*
