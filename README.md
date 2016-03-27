alpine-go-builder
=================

A builder image to build go code. It's based in alpine-base.

## Build

```
docker build -t rawmind/alpine-go-builder:<version> .
```

## Versions

- `0.3.3` [(Dockerfile)](https://github.com/rawmind0/alpine-go-builder/blob/master/Dockerfile)

## Usage

To use this image, run it with a build script as a parameter. A build script must have all the commands to build your app.

```
docker run  -t --rm \
       -v <code-path>:/opr/src/<app> \
       alpine-go-builder:<version> ./build.sh"
```

