[![Build Status](https://travis-ci.org/aignas/shed.svg?branch=master)](https://travis-ci.org/aignas/shed)
[![aignas/shed container status](https://images.microbadger.com/badges/image/aignas/shed.svg)](https://microbadger.com/images/aignas/shed "Docker image badger from microbadger.com")

# Toolshed

[aignas/shed](https://hub.docker.com/r/aignas/shed/) is a docker
image with many command-line tools.

# Usage

Setup:
```sh
$ grep -A3 shed ~/.zshrc
shed() {
    docker run --name shed -v `pwd`:/x -w /x -ti --rm aignas/shed "$@"
}
```

The above will execute the shed with `/x/` mounted as the current directory.

## A few examples

A Bash prompt in a rich environment:
```sh
$ shed
```
