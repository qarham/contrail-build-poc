# Contrail build system POC

## Design

The design can be found in the following doc:
https://docs.google.com/document/d/10QZigXMjsujC23fp-y239iK5a7r05UhBW95uybvqJtc/edit#

## Prerequisites

This is tested on CentOS 7.4

## How to use

At first you need to update kernel and reboot. Because reboot is not possible in the middle of the process.
```
  yum -y install epel-release
  yum -y update
  yum -y install kernel-devel kernel-headers
  reboot
```

Then just clone this repo and run build.sh.
It should run all steps and build RPM-s.
Last step will build docker images from build RPM-s.
