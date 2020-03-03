# RandomLinuxUtilities

This repository contains some random Linux utilities I plan to create. I will start with some simple files, for viewing process load on the go etc. Please feel free to fork and contribute and improve my code as you see fit.

These are the scripts I have loaded so far.

### rtload

This is a simple script which displays a single-line progress bar. This bar shows the queuing load of the processors. It updates automatically after every three seconds. I will provide detailed documentation in the future.

This script uses a shebang and not a file extension. This is because it is meant to be used as a command. Put it in your PATH location, preferably into a local location inside `$HOME/.local/`.

`rtload` is a command meant to be used on split-screen terminals like Terminator. Simply type the command `rtload` to start, and use the `Ctrl+C` interrupt to end it.

**Dependencies:** `rtload` requires the commands `w` and `bc` to run. These should come preinstalled with the Linux Kernel, since they are both components of the *GNU-coreutils* package. Additionally, it runs on `/usr/bin/env bash`, so change the shebang to your prefered shell if you use a different shell (you probably don't).

### brailleimg

This is a Python (v3) script which implements a command to convert raster images into Unicode textfiles. For more details, use `brailleimg --help` after putting the script inside your `$PATH`. The script is POSIX-compliant.

**Dependencies:** `brailleimg` requires Python3 to work. It also makes use of the Numpy and Scikit-Image packages, which can be installed using the commands:
```
pip3 install --user numpy
pip3 install --user scikit-image
```

*NOTE: `bangla` is not a complete script. I will update the README.md after adding more to it.*

### CSView

The file `csview` is a simple utility for viewing CSV files in neatly formatted tables inside the terminal. It runs on Python3. Just place the file inside your `PATH` and make sure that your Python3 is located in `/usr/bin/`. You can check this using `which python3`. If Python3 is located somewhere else, modify the first line of this file to the address of Python3, which is printed as the output of the `which python3` command.

#### TODO:
  [ ] complete the script Bangla - add *juktakkhor*.  
  [ ] implement BASH colors into brailleimg  
  [ ] write a --help option for rtload  
