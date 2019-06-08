# shearch

shearch is a simple wrapper around find, providing a GTK interface.
It is mostly meant to be used as a custom action of your file manager.

## Install

Either copy the script and the manpage somewhere in your path and
manpath respectively, or use the provided install script which will
install both under /usr/local/bin and /usr/local/share/man/man1/ by
running:
- sudo ./install

If you wish to install under a different prefix, provided you have
the required rights, provide it as an argument, like so:
- ./install "path/to/my/dir"

## Uninstall

In complete parallel to install, run:
- sudo ./uninstall
or, if you installed under a different prefix
- ./uninstall "path/to/my/dir"

## Example

Usage is fairly simple, just execute **shearch** and you're done. To integrate
with a file manager such as Thunar you can create a custom action with the
following command **shearch -d %f** and set it to appear when the selection
contains directories.
