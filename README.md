# cppcraft

me just futzing around in bgfx doing random things :)

## How 2 build?

Only works on macOS right now,
because `build.zig` always builds
macOS extensions like Metal and whatnot.

Note that you must have [zigmod](https://nektro.github.io/zigmod/)
installed to build this program.

```shell
# build the shader compiler
cd dependencies/bgfx
make shaderc texturec

# build shaders & textures
cd ../../
./build_resources.sh

# build & run the program
git clone git@github.com:crockeo/cppcraft
cd cppcraft
git submodule update --init --recursive
zigmod fetch
zig build run
```
