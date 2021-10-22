## SmallerC

A small C compiler written in Python. Generates x64 Intel-format assembly, which is then assembled and linked by `nasm` and `ld`.

### Features

See the `tests` folder for examples that compile. The `function_test.c` test is representative of the range of SmallerC.

- Math
  - Operations: `+`, `-`, `*`, `/`, `%`, `++`, `--`, `&&`, `||`, `!`
  - Assignment: `=`, `+=`, `-=`, `*=`, `/=`, `%=`
  - Comparison: `==`, `!=`, `<`, `<=`, `>`, `>=`
- `int` type variables
- Control structures:
  - `if`
  - `while`
  - `for`
  - `break`
  - `continue`
- Pointers (referencing and dereferencing)
- Arrays
- Function definition and calling
- `\* ... */`-form comments
- `print` statement: `print n` outputs the integer `n` to stdout.
  - This isn't in the C spec, but I included it to facilitate outputting values from the program; SmallerC is nowhere near being able to compile the stdio C libraries.