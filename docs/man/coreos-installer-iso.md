---
layout: default
parent: Command line reference
nav_order: 4
---

# coreos-installer iso

## Description

Commands to manage a CoreOS live ISO image

## Usage

* coreos-installer iso &lt;SUBCOMMAND&gt;

## Subcommands

* ignition  Embed an Ignition config in a CoreOS live ISO image

# coreos-installer iso ignition

## Description

Embed an Ignition config in a CoreOS live ISO image

## Usage

* coreos-installer iso ignition &lt;SUBCOMMAND&gt;

## Subcommands

* embed  Embed an Ignition config in an ISO image
* show  Show the embedded Ignition config from an ISO image
* remove  Remove an existing embedded Ignition config from an ISO image

# coreos-installer iso ignition embed

## Description

Embed an Ignition config in an ISO image

## Usage

* coreos-installer iso ignition embed [OPTIONS] &lt;ISO&gt;

## Options

* **-f**, **--force**  Overwrite an existing Ignition config
* **-i**, **--ignition-file** &lt;path&gt;  Ignition config to embed [default: stdin]
* **-o**, **--output** &lt;path&gt;  Write ISO to a new output file

## Arguments

* &lt;ISO&gt;  ISO image

# coreos-installer iso ignition show

## Description

Show the embedded Ignition config from an ISO image

## Usage

* coreos-installer iso ignition show &lt;ISO&gt;

## Arguments

* &lt;ISO&gt;  ISO image

# coreos-installer iso ignition remove

## Description

Remove an existing embedded Ignition config from an ISO image

## Usage

* coreos-installer iso ignition remove &lt;ISO&gt;

## Options

* **-o**, **--output** &lt;path&gt;  Copy to a new file, instead of modifying in place

## Arguments

* &lt;ISO&gt;  ISO image
