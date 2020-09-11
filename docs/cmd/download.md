---
layout: default
parent: Command line reference
nav_order: 2
---

# coreos-installer download

## Description

Download a CoreOS image

## Usage

**coreos-installer download** [*options*]

## Options

**--stream**, **-s** *name*

Fedora CoreOS stream [default: stable]

**--architecture** *name*

Target CPU architecture [default: x86_64]

**--platform**, **-p** *name*

Fedora CoreOS platform name [default: metal]

**--format**, **-f** *name*

Image format [default: raw.xz]

**-u**, **--image-url** *URL*

Manually specify the image URL

**--directory**, **-C** *path*

Destination directory [default: .]

**--decompress**, **-d**

Decompress image and don't save signature

**--insecure**

Skip signature verification

**--stream-base-url** *URL*

Base URL for Fedora CoreOS stream metadata
