# Mojo's libc support

![logo](./assets/logo.jpeg)

`mojo-libc` is a library that provides access to the C standard library functions in Mojo.

## Getting Started

The only dependency for `libc` is Mojo.

You can install Mojo following the instructions from the [Modular website](https://www.modular.com/max/mojo).

Once you have created a Mojo project using the `magic` tool,

### If you are using the magic CLI

Install the `libc` library by running the following command:

```bash
magic add libc
```

### If you have a Mojo project with a `toml` file

1. Add the `libc` dependency to your `toml` file, e.g:
   ```toml
   [dependencies]
   libc = ">=0.1.13"
   ```
3. Run `magic install` at the root of your project, where the `toml` file is located
4. `libc` should now be installed as a dependency. You can import libc functions from the library, e.g:
    ```mojo
    from libc import socket
    ```

## Supported Functionality

### Basic socket connections

See the examples in [examples/sockets/](examples/sockets/) directory.

### Basic file system operations

See the examples in [examples/files/](examples/files/) directory.

## Building the project

To build the project, execute the following command:

```bash
./scripts/build.sh
```

## Running the tests

To run the tests, execute the following command:

```bash
./scripts/run-tests.sh
```
