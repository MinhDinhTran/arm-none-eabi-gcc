[![Github All Releases](https://img.shields.io/github/downloads/gnu-mcu-eclipse/arm-none-eabi-gcc/latest/total.svg)](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases/) [![Github All Releases](https://img.shields.io/github/downloads/gnu-mcu-eclipse/arm-none-eabi-gcc/total.svg)](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases/)

# GNU MCU Eclipse ARM Embedded GCC

## Rationale

**GNU MCU Eclipse ARM Embedded GCC** is a new GCC toolchain distribution 
for ARM devices, that complements the official 
[GNU Arm Embedded Toolchain](https://developer.arm.com/open-source/gnu-toolchain/gnu-rm)
distribution, by ARM.

For main benefits for the users are:

- convenience: binaries for all major platforms are provided 
(Windows 64/32-bit, GNU/Linux 64/32-bit, macOS); 
- uniform and portable install: the toolchain is also available 
as a binary xPack, and can be easily installed with `xpm`;
- improved support for Continuous Integration usage: 
as for any xPack, the toolchain can be easily used
in test environments.

## Changes

Compared to the original ARM release, there are no functional changes; 
the **same architecture options** are supported, and **the same 
combinations of libraries** (derived from newlib) are provided.


## Releases

The **GNU MCU Eclipse ARM Embedded GCC** releases generally follow the official 
[GNU Arm Embedded Toolchain](https://developer.arm.com/open-source/gnu-toolchain/gnu-rm) 
releases, maintained by ARM.

### 8.2.1-1.4 (2019-02-14)

This release is functionally equivalent to **8-2018-q4-major** from December 20, 2018, 
and is based on `gcc-arm-none-eabi-8-2018-q4-major-src.tar.bz2`
([download](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases/tag/v8.2.1-1.2)),
but fixes the bugs present in the initial ARM release.

### 8.2.1-1.1 (2019-01-02)

This release is functionally equivalent to **8-2018-q4-major** from December 20, 2018, 
and is based on `gcc-arm-none-eabi-8-2018-q4-major-src.tar.bz2`
([download](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases/tag/v8.2.1-1.1)).

### 7.3.1-1.1 (2018-07-24)

This release is functionally equivalent to **7-2018-q2-update** from June 27, 2018, 
and is based on `gcc-arm-none-eabi-7-2018-q2-update-src.tar.bz2`
([download](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases/tag/v7.3.1-1.1)).

There should be no changes compared to the ARM release.

### 7.2.1-1.1 (2018-04-01)

This release is functionally equivalent to **7-2017-q4-major** from December 18, 2017, 
and is based on `gcc-arm-none-eabi-7-2017-q4-major-src.tar.bz2`
([download](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases/tag/v7.2.1-1.1)).

The only changes are small improvements to newlib, which was extended with 
`--enable-newlib-io-c99-formats` to enable C99 support in IO functions 
like printf/scanf. This option does not affect newlib-nano.

### 6.3.1-1.1 (2018-03-31)

This release is functionally equivalent to **6-2017-q2-update** from June 28, 2017,
and is based on `gcc-arm-none-eabi-6-2017-q2-update-src.tar.bz2`
([download](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases/tag/v6.3.1-1.1)).

The only changes are small improvements to newlib, which was extended with 
`--enable-newlib-io-c99-formats` to enable C99 support in IO functions 
like printf/scanf. This option does not affect newlib-nano.

## Install

The procedure to install **GNU MCU Eclipse ARM Embedded GCC** is platform 
specific, but relatively straight forward (a .zip archive on Windows, 
a compressed tar archive on macOS and GNU/Linux).

A portable method is to use [`xpm`](https://www.npmjs.com/package/xpm):

```console
$ xpm install @gnu-mcu-eclipse/arm-none-eabi-gcc --global
```

More details are available on the 
[How to install the ARM toolchain?](https://gnu-mcu-eclipse.github.io/toolchain/arm/install/) 
page.

## Build

The build scripts are part of the separate 
[gnu-mcu-eclipse/arm-none-eabi-gcc-build](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc-build)
project.

This project does not include any source files, the build scripts use the 
_Source Invariant_ archives provided by ARM.

## Publish

The procedure used to publish the binaries is documented in the separate
[PUBLISH](PUBLISH.md) page.

The metadata files used to publish the xPacks on the `npmjs.com` server 
are available from the 
[gnu-mcu-eclipse/arm-none-eabi-gcc-xpack](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc-xpack)
project.

## Download analytics

* GitHub [gnu-mcu-eclipse/arm-none-eabi-gcc.git](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/)
  * latest release
[![Github All Releases](https://img.shields.io/github/downloads/gnu-mcu-eclipse/arm-none-eabi-gcc/latest/total.svg)](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases/)
  * all releases [![Github All Releases](https://img.shields.io/github/downloads/gnu-mcu-eclipse/arm-none-eabi-gcc/total.svg)](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases/)
* xPack [@gnu-mcu-eclipse/arm-none-eabi-gcc](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc-xpack/)
  * latest release, per month 
[![npm (scoped)](https://img.shields.io/npm/v/@gnu-mcu-eclipse/arm-none-eabi-gcc.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/arm-none-eabi-gcc/)
[![npm](https://img.shields.io/npm/dm/@gnu-mcu-eclipse/arm-none-eabi-gcc.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/arm-none-eabi-gcc/)
  * all releases [![npm](https://img.shields.io/npm/dt/@gnu-mcu-eclipse/arm-none-eabi-gcc.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/arm-none-eabi-gcc/)
* [individual file counters](https://www.somsubhra.com/github-release-stats/?username=gnu-mcu-eclipse&repository=arm-none-eabi-gcc) (grouped per release)
  
Credit to [Shields IO](https://shields.io) and [Somsubhra/github-release-stats](https://github.com/Somsubhra/github-release-stats).