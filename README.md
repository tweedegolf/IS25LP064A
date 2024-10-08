# IS25LP064A Flash driver

[![crates.io](https://img.shields.io/crates/v/is25lp064a.svg)](https://crates.io/crates/is25lp064a) [![Documentation](https://docs.rs/is25lp064a/badge.svg)](https://docs.rs/is25lp064a)

This is a generic driver for the IS25LP064A flash chip from ISSI.

It supports:
- Blocking SPI using `embedded-hal 1.0`
- Async SPI using `embedded-hal-async`
- Blocking `embedded-storage`
- Async `embedded-storage-async`

To unlock the use of async, activate the `async` feature on the crate.

Defmt is also supported through the `defmt` feature.

## TODO

- Fast read support. So far there's only support for the normal read, so don't use a SPI speed of > 50Mhz

## Changelog

### Unreleased

### [0.1.0] - 2024-10-08
- Initial release (forked from w25q32jv)
  - Increased page count
  - Made unique ID 16 bytes
