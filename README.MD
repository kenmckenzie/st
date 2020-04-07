st - simple terminal
=====================
st is a simple terminal emulator for X which sucks less. This is a custom version with a few added patches


Patches Addded
--------------
font2
rightclicktoplumb
scrollback & scrollback mouse
xresource patch
alpha

Please read the relevent documentation on suckless'es website for more info on the patches and what they do

Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
Please see the config.def.h for all the keybindings, its fairly straightforward 

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
All the original suckless devs

Huge thank you to https://github.com/bakkeby for flexipatch which helped me include all the patches without days of troubleshooting  