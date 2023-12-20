# Install MetaReal

To install MetaReal, you can clone the MetaReal repository and build it according to the instructions.

```bash
$ git clone "https://github.com/Meta-Real/MetaReal.git"
```

## Installation

### Setup On Windows

Download and install [MSYS2](https://www.msys2.org). \
Install gcc, cmake, and make in the MSYS2 mingw64 terminal window.

```bash
$ pacman -S gcc cmake make
```

The rest of the steps are identical between different operating systems.

### MetaReal Installation

Go to the project directory and open up the terminal window (MSYS2 mingw64 terminal window in Windows). \
Create a directory called `build` and open it.

```bash
$ mkdir build
$ cd build
```

Build the project and make it.

```bash
$ cmake ..
$ make
```

Go back to the project directory and run the MetaReal executable file.

```bash
$ cd ..
$ ./MetaReal
```
