# BracketMatching

This is a C++ project that checks if a source code file has balanced brackets, such as "[]", "()", and "{}". It also reports detailed error messages if any mismatch is detected.

## Features

- Implements a templated list data structure and a stack interface
- Uses the catch2 framework for testing and debugging
- Compares the runtime and memory usage of two versions of the stack: one based on a list and one based on a vector
- Handles different types of brackets and string delimiters in C++


Then, navigate to the project directory and run the following commands:

```bash
mkdir build
cd build
cmake ..
make
```

This will generate two executables: `check_brackets_list` and `check_brackets_vector`, which use the list-based and vector-based stack implementations, respectively.

## Usage

To check a source code file for balanced brackets, you can run either of the executables with the file name as an argument. For example:

```bash
./check_brackets_list test_data/test1.cpp
```

The program will output either "OK" or "Bracket mismatch detected", followed by some debugging information if an error is found. The program will also report the runtime in milliseconds.

You can also run the tests for the list and stack classes using the following command:

```bash
./test
```

This will run the catch2 test cases and report the results.
