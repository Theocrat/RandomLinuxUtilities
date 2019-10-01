# RandomLinuxUtilities

This repository contains some random Linux utilities I plan to create. I will start with some simple files, for viewing process load on the go etc. Please feel free to fork and contribute and improve my code as you see fit.

These are the scripts I have loaded so far.

### rtload

This is a simple script which displays a single-line progress bar. This bar shows the queuing load of the processors. It updates automatically after every three seconds. I will provide detailed documentation in the future.

This script uses a shebang and not a file extension. This is because it is meant to be used as a command. Put it in your PATH location, preferably into a local location inside `$HOME/.local/`.

`rtload` is a command meant to be used on split-screen terminals like Terminator. Simply type the command `rtload` to start, and use the `Ctrl+C` interrupt to end it.

**Dependencies:** `rtload` requires the commands `w` and `bc` to run. These should come preinstalled with the Linux Kernel, since they are both components of the *GNU-coreutils* package. Additionally, it runs on `/usr/bin/env bash`, so change the shebang to your prefered shell if you use a different shell (you probably don't).
