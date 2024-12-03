# Application for quickly and securely building encrypted archives.
*Author: Kamil Ciaś, <kamil.cias@nexstep.systems>*

*GPL-3.0 license*
*This script is distributed under the terms of the GNU General Public License, version 3.0 or later.
Details of the license can be found at: [https://www.gnu.org/licenses/gpl-3.0.html](https://www.gnu.org/licenses/gpl-3.0.html)*

## Description:
> The **seclogs** application is used to quickly and safely create encrypted archives in a Linux environment. A script with the -e or --encrypt parameter takes a directory as an argument, packs and compresses it, and then encrypts it. The result of the application is an encrypted and compressed archive. Decryption with the -d or --decrypt parameter involves providing the encrypted file as an argument. The application asks for a password, then decrypts, decompresses and unpacks the given archive into a directory.

> You can use the application both locally and globally. The local call takes place in the current directory, but to use the application globally, you must grant executable rights **chmod +x seclogs** and move the script to the **/usr/bin** location.


## Usage:

seclogs [option] [directory_path]

### For directory encryption
```shell
seclogs [-e|--encrypt] [directory_path]
```
or

### For file decryption *future functionality*
```shell
seclogs [-d|--decrypt] encrypted-file
```
or

### Display help
```shell
seclogs [-h|--help]
```
or

### Version display
```shell
seclogs [-v|--version]
```

## Options
```shell
Usage: seclogs [-e|--encrypt] [-h|--help] [directory_path]
Options:
-e, --encrypt    Encrypt files in the specified directory
-h, --help       Display this help message
-v, --version    Display the app version

```

## Future functionality

> The application will be able to send the password in a safe way, decrypt the package to the indicated location, and select both the type of archive and the compression algorithm.

> For readability of the code, the various functions will go into separate files, and the packages themselves will be generated for popular package managers such as "rpm" or "deb".
