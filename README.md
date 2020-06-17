nightly
=======

nightly builds of select python packages.

for released versions use
[ppa:deadsnakes/ppa](https://launchpad.net/~deadsnakes/+archive/ubuntu/ppa)

## tl;dr

https://launchpad.net/~deadsnakes/+archive/ubuntu/nightly

```bash
sudo add-apt-repository ppa:deadsnakes/nightly
sudo apt update
```

## limitations

these packages are missing a few things to make the builds more automatable

- the documentation build (surprisingly the thing that breaks the most in
  cpython builds)
- the debian libpython symbols tracking (this is really only useful for stable
  packages and building other packages against them -- it also causes a break
  any time upstream adds / removes a symbol).
- the `NEWS` file (this file is only present on releases, hope you don't need
  it!)

## available packages

packages are only built for the amd64 architecture for the following:

- [![Build Status](https://github.com/deadsnakes/python3.7-nightly/workflows/main/badge.svg)](https://github.com/deadsnakes/python3.7-nightly/actions) python3.7 (xenial, bionic)
- [![Build Status](https://github.com/deadsnakes/python3.8-nightly/workflows/main/badge.svg)](https://github.com/deadsnakes/python3.8-nightly/actions) python3.8 (xenial, bionic)
- [![Build Status](https://github.com/deadsnakes/python3.9-nightly/workflows/main/badge.svg)](https://github.com/deadsnakes/python3.9-nightly/actions) python3.9 (xenial, bionic, focal)
- [![Build Status](https://github.com/deadsnakes/python3.10-nightly/workflows/main/badge.svg)](https://github.com/deadsnakes/python3.10-nightly/actions) python3.10 (xenial, bionic, focal)
