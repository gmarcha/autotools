# autotools
Sample describing autotools usage.

## Usage

- Create and write `configure.ac` in root directory and a `Makefile.am` in root directory and each subdirectory containing source code.
  
- Run `autoreconf --install` to perform configuration files and Makefile/Makefile.in generation\
    (`autoreconf` runs autotools toolchain in right order: `aclocal`, `autoconf`, `autoheader`, `automake`).

- Use `./configure && make && sudo make install` to install package.

- Use `./configure --prefix=/usr` to change installation path.

- Use `make CC=<pathToCompiler> CFLAGS="<compilerFlags>"` to change compiler and compiler options (default to `gcc` and `-g -O2` respectively).

## Links

- Official [documentation](https://www.gnu.org/software/automake/manual/html_node/Autotools-Introduction.html).
- [Slides](https://www.lrde.epita.fr/~adl/dl/autotools.pdf) describing autotools workflow.
