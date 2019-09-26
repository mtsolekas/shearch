# shearch

shearch is a simple wrapper around find, providing a GTK interface.
It is mostly meant to be used as a custom action of your file manager.

## Install

Running the below command will install both executable and manpage
under /usr/local/bin and /usr/local/share/man/man1/:
- sudo make install

If you wish to install under a different prefix, provided you have
the required rights, provide it as an argument, like so:
- make PREFIX="path/to/my/dir" install

## Uninstall

In complete parallel to install, run:
- sudo make uninstall
or, if you installed under a different prefix
- make PREFIX="path/to/my/dir" uninstall

## Example

Usage is fairly simple, just execute **shearch** and you're done. To integrate
with a file manager such as Thunar you can create a custom action with the
following command **shearch -d %f** and set it to appear when the selection
contains directories.
