[![uBlue Build](https://github.com/noconnor29/bluefin-dx/actions/workflows/build.yml/badge.svg)](https://github.com/noconnor29/bluefin-dx/actions/workflows/build.yml)
# Purpose

This repository is meant to be a template for building your own custom Universal Blue image.

This template includes a Containerfile and a Github workflow for building the container image. As soon as the workflow is enabled in your repository, it will build the container image and push it to the Github Container Registry.

# How to Use
## Containerfile

This file defines the operations used to customize the selected image. It contains examples of possible modifications, including how to:
- change the upstream from which the custom image is derived
- add additional RPM packages
- add binaries as a layer from other images

## Workflows

### build.yml

This workflow creates your custom OCI image and publishes it to the Github Container Registry (GHCR). By default, the image name will match the Github repository name.

### Other Examples
- [m2os](https://github.com/m2giles/m2os)
- [bos](https://github.com/bsherman/bos)
- [homer](https://github.com/bketelsen/homer/)
