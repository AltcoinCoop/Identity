## Building Identity

RECOMMENDED set up, Ubuntu 14, g++, cmake, Libboost 1.55-all-dev

From Terminal use: (--> symbol is to show you need to type a command DONT INCLUDE IT) (Same with () those are there to help, dont include them in the command)

--> sudo apt install cmake

--> sudo apt install g++

--> sudo apt install libboost1.55-all-dev

--> sudo apt-get install git

--> git clone https://github.com/IdentityProject/Identity.git (optional add a folder destination otherwise default is Identity)

--> cd (name of folder you created, Default will be Identity)

--> make

(wait for it to compile)

--> cd build/release/src
To run chain (make sure you are in the right directory E.G. Identity/build/release/src)

--> ./identityd

~Congrats you are now running the chain!

~ If you want to mine from here use:

--> start_mining (insert wallet address) (number of cpu)

--> stop_mining

If you need a wallet address look at section below.
To create a wallet on the terminal simply use (make sure you are not still running the chain)

--> ./simplewallet

It will give you the option to Make a new wallet or Open an existing one

Assuming you need a new one use:

--> g

--> name your wallet

--> choose password

Congrats you have your own wallet!

command list use:

--> help

typical commands used

--> address (this shows you your address)

--> start_mining (this starts mining to your wallet)

--> stop_mining (this stops mining)

--> balance (this shows you your balance)

### On *nix:

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.55 or later.

You may download them from:

- http://gcc.gnu.org/
- http://www.cmake.org/
- http://www.boost.org/

Alternatively, it may be possible to install them using a package manager.

To build, change to a directory where this file is located, and run `make`. The resulting executables can be found in `build/release/src`.

#### Advanced options:

Parallel build: run `make -j<number of threads>` instead of `make`.

Debug build: run `make build-debug`.

Test suite: run `make test-release` to run tests in addition to building. Running `make test-debug` will do the same to the debug version.

Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run `export CC=clang CXX=clang++` before running `make`.

### On Windows:
Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, and Boost 1.55 or later. You may download them from:

- http://www.microsoft.com/
- http://www.cmake.org/
- http://www.boost.org/

To build, change to a directory where this file is located, and run this commands:
```
mkdir build
cd build
cmake -G "Visual Studio 12 Win64" ..
```

And then do Build.

Good luck!
