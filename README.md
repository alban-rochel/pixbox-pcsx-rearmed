pixbox-pcsx-rearmed
=========

This is a fork of pcsx-rearmed for my personal Pixbox project: http://pixbox-project.blogspot.fr/

Check the original version of pcsx-rearmed: https://github.com/notaz/pcsx_rearmed
Check the original version of libpicofe: https://github.com/notaz/libpicofe

My changes are documented in pixbox.patch, and the motivation behind these changes are explained on my project page.

Changes are:
* Modification of the configure script to enable the right options for the BeagleBone Black platform with SDL
* Made the base save/configuration path absolute (and hard-coded)
* Removed the menu when setting the NO_MENU environment variable
* Removed a few "if"s that were never used in my case (show fps etc.)
* Modification of the internal libpicofe, so that the environment variable PCSX_WIDTH, when set, allows forcing a size for the display.

Disclaimer
------------

The modified pieces of code were not written in the idea of being distributed, they are provided as-is for the entertainment of whoever could want to try them.
