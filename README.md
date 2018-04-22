[![npm (scoped)](https://img.shields.io/npm/v/@gnu-mcu-eclipse/windows-build-tools.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/windows-build-tools) 
[![license](https://img.shields.io/github/license/gnu-mcu-eclipse/windows-build-tools-xpack.svg)](https://github.com/gnu-mcu-eclipse/windows-build-tools-xpack/blob/xpack/LICENSE) [![npm](https://img.shields.io/npm/dt/@gnu-mcu-eclipse/windows-build-tools.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/windows-build-tools/)


## GNU MCU Eclipse Windows Build Tools binaries

This xPack installs the platform specific binaries for Windows Build Tools.

This project is open source and it is publicly available from [GitHub](https://github.com/gnu-mcu-eclipse/windows-build-tools-xpack).

## How to use

This section is intended for developers who plan to use the Windows Build Tools.

### Prerequisites

A recent [`xpm`](https://www.npmjs.com/package/xpm), which is a 
portable [Node.js](https://nodejs.org/) command line application.

## Easy install

The module is available as [`@gnu-mcu-eclipse/windows-build-tools`](https://www.npmjs.com/package/gnu-mcu-eclipse/windows-build-tools) from the `npmjs.com` registry; with `xpm` available, installing the latest version of the package is quite easy:

```console
$ xpm install @gnu-mcu-eclipse/windows-build-tools --global
```

Global `xpm` packages are installed in the user home folder, and do not require `sudo`.

To remove the installed xPack, the command is similar:

```console
$ xpm uninstall @gnu-mcu-eclipse/windows-build-tools --global
```

(Note: not yet implemented)

## Developer info

### Git repo

```console
$ git clone https://github.com/gnu-mcu-eclipse/windows-build-tools-xpack.git windows-build-tools-xpack.git
```

### Windows Build Tools binaries

The binaries are downloaded from the [gnu-mcu-eclipse/windows-build-tools.git](https://github.com/gnu-mcu-eclipse/windows-build-tools) project, the [releases](https://github.com/gnu-mcu-eclipse/windows-build-tools/releases) page.

### Code standard compliance

The module currently does not include any JavaScript code.

### Code documentation metadata

The module currently does not include any documentation metadata

## Maintainer info

### How to publish

* open [releases](https://github.com/gnu-mcu-eclipse/windows-build-tools/releases) and select the latest release
* update the `baseUrl:` with the file URLs (including the tag/version)
* from the blog post, copy the SHA & file names
* commit all changes, use a message like `2.10.1` (without `v`)
* `npm version 2.10.1`
* push all changes to GitHub
* `npm publish`

## License

The original content is released under the [MIT License](https://opensource.org/licenses/MIT), with all rights reserved to [Liviu Ionescu](https://github.com/ilg-ul).
