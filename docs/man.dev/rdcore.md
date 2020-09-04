---
layout: default
parent: Development
---

# rdcore

The `rdcore` binary is not intended to be used directly and is targetted toward
inclusion in an initramfs built via `dracut` to perform specific tasks that are
hard to write in Bash.

## Usage

* rdcore &lt;SUBCOMMAND&gt;

## Subcommands

* rootmap  Generate rootmap kargs and optionally inject into BLS configs
* stream-hash  Copy data from stdin to stdout, checking piecewise hashes

# rdcore rootmap

Generate rootmap kargs and optionally inject into BLS configs

## Usage

* rdcore rootmap &lt;ROOT_MOUNT&gt;

## Options

* **--boot-device** &lt;DEVPATH&gt;  Boot device containing BLS entries to modify
* **--boot-mount** &lt;BOOT_MOUNT&gt;  Boot mount containing BLS entries to modify

## Arguments

* &lt;ROOT_MOUNT&gt;  Path to rootfs mount

# rdcore stream-hash

## Description

Copy data from stdin to stdout, checking piecewise hashes

## Usage

* rdcore stream-hash &lt;hash-file&gt;

## Arguments

* &lt;hash-file&gt;  Path to the piecewise hash file
