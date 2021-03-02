# ubuntu packaging nvidia modprobe

[![License](https://img.shields.io/badge/License-GPL%202.0-blue.svg)](https://opensource.org/licenses/GPL-2.0)
[![Contributing](https://img.shields.io/badge/Contributing-Developer%20Certificate%20of%20Origin-violet)](https://developercertificate.org)

## Overview

Packaging templates for `Ubuntu` based Linux distros to build NVIDIA modprobe packages.

The `main` branch contains this README. The `control` and `.install` files can be found in the appropriate [16.04](../../tree/16.04), [18.04](../../tree/18.04), and [20.04](../../tree/20.04) branches.

## Table of Contents

- [Overview](#Overview)
- [Deliverables](#Deliverables)
- [Prerequisites](#Prerequisites)
  * [Clone this git repository](#Clone-this-git-repository)
  * [Download a NVIDIA modprobe tarball](#Download-a-NVIDIA-modprobe-tarball)
  * [Install build dependencies](#Install-build-dependencies)
- [Related](#Related)
  * [NVIDIA modprobe](#NVIDIA-modprobe)
  * [NVIDIA settings](#NVIDIA-settings)
- [Contributing](#Contributing)


## Deliverables

This repo contains the template files used to build the following **DEB** packages:

```shell
- nvidia-modprobe
```
> *note:* this package does not support "flavor" / locking to a specific driver branch.

## Prerequisites

### Clone this git repository:

Supported branches: `16.04`, `18.04` & `20.04`

```shell
git clone -b ${branch} https://github.com/NVIDIA/ubuntu-packaging-nvidia-modprobe
> ex: git clone -b 18.04 https://github.com/NVIDIA/ubuntu-packaging-nvidia-modprobe
```

### Download a NVIDIA modprobe tarball:

* **Source code** location: [https://github.com/NVIDIA/nvidia-modprobe/releases](https://github.com/NVIDIA/nvidia-modprobe/releases)

  *ex:* [https://github.com/NVIDIA/nvidia-modprobe/archive/460.32.03.tar.gz](https://github.com/NVIDIA/nvidia-modprobe/archive/460.32.03.tar.gz)

  *ex:* [https://github.com/NVIDIA/nvidia-modprobe/archive/460.56.tar.gz](https://github.com/NVIDIA/nvidia-modprobe/archive/460.56.tar.gz)

### Install build dependencies
> *note:* these are only needed for building not installation

```shell
# Packaging
apt-get install debhelper devscripts dpkg-dev
```

## Related

- nvidia-driver
  * [https://github.com/NVIDIA/ubuntu-packaging-nvidia-driver](https://github.com/NVIDIA/ubuntu-packaging-nvidia-driver)

- nvidia-settings
  * [https://github.com/NVIDIA/ubuntu-packaging-nvidia-settings](https://github.com/NVIDIA/ubuntu-packaging-nvidia-settings)


## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md)
