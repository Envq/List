# List

This is my implementation of List with LinkedList for the C ++ course

## Table of Contents

* [Getting started](#getting-started)
  * [Dependencies](#dependencies)
  * [Building from source](#building-from-source)
  * [Installing](#installing)
  * [Running tests](#test)
  * [Using tools](#tools)
* [Author](#author)
* [License](#license)

## Getting Started

This code was tested on Ubuntu 18.04 with GCC

### Dependencies

A compiler with C++14 support (clang-3.4+, gcc-5.1+), cmake 3.1+, (git)

~~~
$ sudo apt install clang cmake git
~~~

**Optional dependencies:**

- `doxygen` *required for generating documentation* 
- `clang-format 6.0` *required for formatting code* 
- `clang-tidy` *required for using a linter* 
- `scan-build` *required for static analysis* 
- `cloc` *required for counting lines of code* 
- `valgrind` *required for detecting many memory management and threading bugs* 
- `lizard` *required for cyclomatic complexity analysis* 

~~~
$ sudo apt install doxygen clang-format clang-tidy clang-tools cloc valgrind
$ sudo apt install python-pip
$ pip install lizard
~~~

### Building from source

Run this:

~~~
$ git clone https://github.com/Envq/List.git
$ cd List
$ mkdir -p build
$ cd build
$ cmake ..
$ make
~~~

There's also a helper script available in the root folder:

  ~~~ sh
  $ ./build.sh
  ~~~

### Installing

After building project run:

~~~
$ make install-lib
~~~


### Running tests

After building project run:

~~~
$ make test
$ ./list_test
~~~

### Using tools

After building project:
- To clean 
~~~
$ make clean-all
~~~
- To count line 
~~~
$ make stats
~~~
- To analyze clyclomatic complexity 
~~~
$ make cyclo
~~~
- To generate documentation 
~~~
$ make doc
~~~
- To format code 
~~~
$ make format
~~~

Only for clang building:
- To static scan 
~~~
$ make scan
~~~
- To use linter 
~~~
$ make tidy
~~~

## Author

**Enrico Sgarbanti** [**@Envq**](https://github.com/Envq) <br>
id: VR408621

## License

This project is licensed under the GPL v3 License - see the [LICENSE.md](LICENSE.md) file for details