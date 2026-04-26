# Project README

## Overview
- The project appears to be a C/C++ application named "Gui_GeoGebra2_2" that can be built for multiple platforms including Linux, Windows, Wine, and WebAssembly. It includes source files in the `src` directory and build configuration files (`Makefile.linux`, `Makefile.windows`, `Makefile.wine`, `Makefile.web`).

## Features
- The project is set up to compile with GCC and Clang.
- It uses Make as a build tool.
- Libraries such as X11, png, jpeg, user32, gdi32, winmm, and SDL are mentioned in the build configurations.

## Project Structure
### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries needed: X11, png, jpeg, WINAPI, user32, gdi32, winmm

## Build & Run
- **Linux**: To build for Linux, navigate to the project directory and run:
  ```sh
  make -f Makefile.linux all
  ```
  To execute:
  ```sh
  make -f Makefile.linux exe
  ```

- **Windows**: To build for Windows, use:
  ```sh
  make -f Makefile.windows all
  ```
  To execute:
  ```sh
  make -f Makefile.windows exe
  ```

- **Wine**: To build for Wine (Linux cross compile for Windows), run:
  ```sh
  make -f Makefile.wine all
  ```
  To execute using WINE:
  ```sh
  make -f Makefile.wine exe
  ```

- **WebAssembly**: To build for WebAssembly, use:
  ```sh
  make -f Makefile.web all
  ```
  To run the project in a web browser:
  ```sh
  make -f Makefile.web exe
  ```

- **Build Options**:
  - `make -f Makefile.(os) all` – builds output
  - `make -f Makefile.(os) do` – build + executable output
  - `make -f Makefile.(os) clean` – removes build artifacts