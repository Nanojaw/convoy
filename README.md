# convoy
A more flexible rust build system

The idea is to allow the user to specify how different crates are built in order to speed up compilation time and 
runtime speed by building some crates in release mode

Inspired by C++ build systems such as CMake, Meson and Bazel

### Needed
- convoy needs some sort of configuration language, either an existing one or a DSL
- convoy has to download crates itself from crates.io (https://www.pietroalbini.org/blog/downloading-crates-io/)
- convoy needs to call rustc itself in order to have full control over the build
- convoy needs to resolve dependencies and includes