# Manylinux

This repository is used to build images derived from
https://github.com/pypa/manylinux that include newer versions of GCC pre-baked.

You can find pre-built images at
https://hub.docker.com/r/tktechdocker/manylinux.

You'll likely need to update your build steps to include at least the
following, changing the path for the version of GCC you're using:

```
export CFLAGS="-static-libstdc++"
export CC=/usr/local/gcc-8.3.0/bin/gcc-8.3.0
export CXX=/usr/local/gcc-8.3.0/bin/g++-8.3.0
```
