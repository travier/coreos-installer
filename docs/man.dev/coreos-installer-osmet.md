---
layout: default
parent: Development
---

# coreos-installer osmet

## Description

Efficient CoreOS metal disk image packing using OSTree commits

## Usage

* coreos-installer osmet &lt;SUBCOMMAND&gt;

## Subcommands

* pack  Create osmet file from CoreOS block device
* unpack  Generate raw metal image from osmet file and OSTree repo
* fiemap  Print file extent mapping of specific file

# coreos-installer osmet pack

## Description

Create osmet file from CoreOS block device

## Usage

* coreos-installer osmet pack [OPTIONS] &lt;DEV&gt; **--checksum** &lt;SHA256&gt; **--description** &lt;TEXT&gt; **--output** &lt;FILE&gt;

## Options

* **--output** &lt;FILE&gt;  Path to osmet file to write
* **--checksum** &lt;SHA256&gt;  Expected SHA256 of block device
* **--description** &lt;TEXT&gt;  Description of OS
* **--real-rootdev** &lt;PATH,OFFSET&gt;  Underlying device for e.g. RHCOS LUKS container; _/dev/disk/by-label/root_ should
  be mountable
* **--fast**  Use worse compression, for development builds

## Arguments

* &lt;DEV&gt;  Source device

# coreos-installer osmet unpack

## Description

Generate raw metal image from osmet file and OSTree repo

## Usage

* coreos-installer osmet unpack &lt;PATH&gt; &lt;DEV&gt; **--osmet** &lt;PATH&gt;

## Options

* **--osmet** &lt;PATH&gt;  osmet file

## Arguments

* &lt;PATH&gt;  OSTree repo
* &lt;DEV&gt;  Destination device

# coreos-installer osmet fiemap

## Description

Print file extent mapping of specific file

## Usage

* coreos-installer osmet fiemap &lt;PATH&gt;

## Arguments

* &lt;PATH&gt;  File to map
