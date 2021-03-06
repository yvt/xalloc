# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.7] - 2020-12-09

- Get rid of illegal uses of `std::mem::uninitialized`, replacing them with `MaybeUninit`

## [0.2.6] - 2019-02-28

- Add `Ring::dealloc_front_until` and `Ring::dealloc_back_until`

## [0.2.5] - 2018-12-05

- Add `Ring`, a circular memory allocator
- Wrap `allow(clippy::*)` with `cfg_attr(feature = "cargo-clippy", ...)` in order to make it compatible with the current stable toolchain

## [0.2.4] - 2018-11-07

- Fix a compilation issue that happens when multiple versions of `num-*` crates are mixed up
- Optimize for performance through a use of the `unreachable` crate and an architecture-specific micro-tuning

## [0.2.3] - 2018-04-02

- Use `std::ptr::NonNull` stabilized in [Rust 1.25]

[Rust 1.25]: https://blog.rust-lang.org/2018/03/29/Rust-1.25.html

## [0.2.2] - 2017-10-28

- Make more types `Debug`
- Add type aliases `SysTlsfRegion` and `SafeTlsfRegion`

## [0.2.1] - 2017-10-28

- Fix a link in `README.md`

## [0.2.0] - 2017-10-28

- Rename `TlsfSuballocRegion` to `TlsfRegion`.
- Add a free space bitmap-based allocator.
- Add CHANGELOG to track notable changes among versions.

## 0.1.0 - 2017-10-28

- Initial release.

[Unreleased]: https://github.com/yvt/xalloc-rs/compare/v0.2.7...HEAD
[0.2.7]: https://github.com/yvt/xalloc-rs/compare/v0.2.6...v0.2.7
[0.2.6]: https://github.com/yvt/xalloc-rs/compare/v0.2.5...v0.2.6
[0.2.5]: https://github.com/yvt/xalloc-rs/compare/v0.2.4...v0.2.5
[0.2.4]: https://github.com/yvt/xalloc-rs/compare/v0.2.3...v0.2.4
[0.2.3]: https://github.com/yvt/xalloc-rs/compare/v0.2.2...v0.2.3
[0.2.2]: https://github.com/yvt/xalloc-rs/compare/v0.2.1...v0.2.2
[0.2.1]: https://github.com/yvt/xalloc-rs/compare/v0.2.0...v0.2.1
[0.2.0]: https://github.com/yvt/xalloc-rs/compare/v0.1.0...v0.2.0
