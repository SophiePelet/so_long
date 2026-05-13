SO_LONG

Overview
--------
`so_long` is a small 2D project from 42 that implements a simple collectible/exit game using MiniLibX.

Important compatibility note
----------------------------
**⚠️ WARNING: This project will not work with the current MiniLibX submodule.**

This code was developed on Ubuntu against the original 42 school MiniLibX version. The repository now includes MiniLibX as a Fedora-compatible submodule, but this newer version is **incompatible** with the codebase. The project was tuned for Ubuntu's MiniLibX API and build setup.

If you wish to use this project, you would need to either:
- Revert to the Ubuntu version of MiniLibX (not included)
- Refactor the code to work with the Fedora MiniLibX (non-trivial)

Requirements (Ubuntu/Debian)
----------------------------
- A C compiler (gcc/clang)
- `make`
- X11 development headers: `libx11-dev`, `libxext-dev`, `libbsd-dev`, `libxrandr-dev`

Building (Ubuntu/Debian)
------------------------
Install dependencies:

```sh
sudo apt update
sudo apt install build-essential libx11-dev libxext-dev libbsd-dev libxrandr-dev
```

Then build the project:

```sh
make
```

Running
-------
After successful build, run the program with a map:

```sh
./so_long maps/map1.ber
```

Maps
----
Maps are in the `maps/` folder. Use the example maps as templates for creating your own `.ber` files.

Troubleshooting
---------------
- Ensure `libX11` and `libXext` are installed: `sudo apt install libx11-dev libxext-dev`
- Verify compilation with `make clean && make` to rebuild from scratch
- This project is only tested and compatible with Ubuntu/Debian-based systems

Contributing / Credits
----------------------
This is a 42 school project. The bundled `mlx_linux/` was cloned from 42 school's repository and is designed for Ubuntu systems.
