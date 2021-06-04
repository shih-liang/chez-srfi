# Introduction

SRFI Package for Chez Scheme of Arch Linux. Prebuilt Packages can be downloaded at [release](https://github.com/shih-liang/chez-srfi/releases).

This is a minor modification of the SRFI collection available at
https://github.com/arcfide/chez-srfi (itself derived from
https://launchpad.net/scheme-libraries).  The modifications are aimed
at improving the integration with Chez Scheme's interactive
environment.

See srfi/README for the original description.

# Install Instructions

`yaourt -S chez-srfi`

# Usage

Example:
```
> (library-directories "/usr/lib/csv9.5.4-site/")
> (import (srfi :42 eager-comprehensions))
> (list-ec (: i 5) (* i i))
(0 1 4 9 16)
```
