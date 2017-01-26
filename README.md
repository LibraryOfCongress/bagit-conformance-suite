# BagIt Conformance Suite

This is a simple collection of BagIt format test cases for different implementations.

## Structure

* The top level of the repository contains directories for each version of the BagIt RFC, prefixed with "v"
* Each version directory should contain a directory named “valid” containing bag directories which must pass validation
  and "invalid" containing bag directories which must fail validation. It may also have a "warning" directory that
  are still valid but should produce a warning.
* Each of the lower level directories should contain a human-meaningful name indicating the aspect being
  tested

## Notes

* Git's `core.autocrlf` setting can cause bag validation failures by converting CRLF files automatically
  depending on your operating system and configuration. It is recommended that you disable it in your local
  checkout of this repository:

  `git config core.autocrlf false`

## License

This repository is released as a [public domain work of the U.S. Government](LICENSE.md).

Contributions are gladly accepted but must be released into the public domain.
