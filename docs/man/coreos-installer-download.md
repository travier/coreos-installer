---
layout: default
parent: Command line reference
nav_order: 2
---

# coreos-installer download

## Description

Download a CoreOS image

## Usage

* coreos-installer download [OPTIONS]

## Options

* **-s**, **--stream** &lt;name&gt; Fedora CoreOS stream [default: stable]
* **--architecture** &lt;name&gt; Target CPU architecture [default: x86_64]
* **-p**, **--platform** &lt;name&gt; Fedora CoreOS platform name [default: metal]
* **-f**, **--format** &lt;name&gt; Image format [default: raw.xz]
* **-u**, **--image-url** &lt;URL&gt; Manually specify the image URL
* **-C**, **--directory** &lt;path&gt; Destination directory [default: .]
* **-d**, **--decompress** Decompress image and don't save signature
* **--insecure** Skip signature verification
* **--stream-base-url** &lt;URL&gt; Base URL for Fedora CoreOS stream metadata
