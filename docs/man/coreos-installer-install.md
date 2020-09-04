---
layout: default
parent: Command line reference
nav_order: 1
---

# coreos-installer install

## Description

Install Fedora CoreOS or RHEL CoreOS

## Usage

* coreos-installer install [OPTIONS] &lt;device&gt;

## Options

* **-s**, **--stream** &lt;name&gt;  Fedora CoreOS stream
* **-u**, **--image-url** &lt;URL&gt;  Manually specify the image URL
* **-f**, **--image-file** &lt;path&gt;  Manually specify a local image file
* **-i**, **--ignition-file** &lt;path&gt;  Embed an Ignition config from a file
* **-I**, **--ignition-url** &lt;URL&gt;  Embed an Ignition config from a URL
* **--ignition-hash** &lt;digest&gt;  Digest (type-value) of the Ignition config
* **-p**, **--platform** &lt;name&gt;  Override the Ignition platform ID
* **--append-karg** &lt;arg&gt;...  Append default kernel arg
* **--delete-karg** &lt;arg&gt;...  Delete default kernel arg
* **-n**, **--copy-network**  Copy network config from install environment
* **--network-dir** &lt;path&gt;  For use with **-n**. [default: /etc/NetworkManager/system-connections/]
* **--save-partlabel** &lt;lx&gt;...  Save partitions with this label glob
* **--save-partindex** &lt;id&gt;...  Save partitions with this number or range
* **--offline**  Force offline installation
* **--insecure**  Skip signature verification
* **--insecure-ignition**  Allow Ignition URL without HTTPS or hash
* **--stream-base-url** &lt;URL&gt;  Base URL for Fedora CoreOS stream metadata
* **--architecture** &lt;name&gt;  Target CPU architecture [default: x86_64]
* **--preserve-on-error**  Don't clear partition table on error

## Arguments

* &lt;device&gt;  Destination device
