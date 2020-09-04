---
layout: default
parent: Command line reference
nav_order: 5
---

# coreos-installer pxe

## Description

Commands to manage a CoreOS live PXE image

## Usage

**coreos-installer pxe** *subcommand*

## Subcommands

**ignition**

Commands to manage a live PXE Ignition config

# coreos-installer pxe ignition

## Description

Commands to manage a live PXE Ignition config

## Usage

**coreos-installer pxe ignition** *subcommand*

## Subcommands

**wrap**

Wrap an Ignition config in an initrd image

**unwrap**

Show the wrapped Ignition config in an initrd image

# coreos-installer pxe ignition wrap

## Description

Wrap an Ignition config in an initrd image

## Usage

**coreos-installer pxe ignition wrap**

## Options

**--ignition-file**, **-i** *path*

Ignition config to wrap [default: stdin]

**--output**, **-o** *path*

Write to a file instead of stdout

# coreos-installer pxe ignition unwrap

## Description

Show the wrapped Ignition config in an initrd image

## Usage

**coreos-installer pxe ignition unwrap** *initrd*

## Arguments

**initrd**

initrd image
