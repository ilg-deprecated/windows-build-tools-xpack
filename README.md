[![npm (scoped)](https://img.shields.io/npm/v/@gnu-mcu-eclipse/windows-build-tools.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/windows-build-tools) 
[![license](https://img.shields.io/github/license/gnu-mcu-eclipse/windows-build-tools-xpack.svg)](https://github.com/gnu-mcu-eclipse/windows-build-tools-xpack/blob/xpack/LICENSE) 
[![npm](https://img.shields.io/npm/dt/@gnu-mcu-eclipse/windows-build-tools.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/windows-build-tools/)


## The GNU MCU Eclipse Windows Build Tools binary xPack

This binary xPack installs the platform specific binaries for
[GNU MCU Eclipse Windows Build Tools](https://github.com/gnu-mcu-eclipse/windows-build-tools).

The source files of the xPack project are publicly available from 
[GitHub](https://github.com/gnu-mcu-eclipse/windows-build-tools-xpack).

## How to use

This section is intended for developers who plan to use the 
Windows Build Tools.

### Prerequisites

The only requirement is a recent 
`xpm`, which is a portable 
[Node.js](https://nodejs.org) command line application. To install it,
follow the instructions from the 
[`xpm`](https://www.npmjs.com/package/xpm) page.

### Easy install

The xPack is available as 
[`@gnu-mcu-eclipse/windows-build-tools`](https://www.npmjs.com/package/gnu-mcu-eclipse/windows-build-tools)
from the public `npmjs.com` repository; with `xpm` available, installing 
the latest version of the package is quite easy:

```console
$ xpm install @gnu-mcu-eclipse/windows-build-tools --global
```

Global xPacks are always installed in the user home folder, even on GNU/Linux  
or macOS, and do not require `sudo`.

The GNU MCU Eclipse plug-ins automatically identify binaries installed with
`xpm` and provide a convenient method to manage paths.

To remove the installed xPack, the command is similar:

```console
$ xpm uninstall @gnu-mcu-eclipse/windows-build-tools --global
```

(Note: not yet implemented. As a temporary workaround, simply remove the 
`xPacks/@gnu-mcu-eclipse/windows-build-tools` folder, or the versions subfolders.)


## Developer info

### The xPack git repo

The few xPack source files are available from GitHub:

```console
$ git clone https://github.com/gnu-mcu-eclipse/windows-build-tools-xpack.git windows-build-tools-xpack.git
```

### Binary files

The binaries are not stored on the `npmjs.com` server, but are downloaded from  
the [releases](https://github.com/gnu-mcu-eclipse/windows-build-tools/releases) 
section of the `gnu-mcu-eclipse/windows-build-tools` GitHub project.

## Maintainer info

### How to publish

* open [releases](https://github.com/gnu-mcu-eclipse/windows-build-tools/releases) 
and select the latest release
* update the `baseUrl:` with the file URLs (including the tag/version)
* from the blog post, copy the SHA & file names
* commit all changes, use a message like `2.10.1` (without `v`)
* update `CHANGELOG.md`; commit with a message like _CHANGELOG: prepare v0.1.2_
* `npm version 2.10.1`
* push all changes to GitHub
* `npm publish`

## License

The original content is released under the 
[MIT License](https://opensource.org/licenses/MIT), with all rights 
reserved to [Liviu Ionescu](https://github.com/ilg-ul).

The binary distributions include several open-source components; the
corresponding licenses are available in the `licenses`
folder.
