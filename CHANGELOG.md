# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.7.1]
### Changed
- Update webpack from 2.1.0-beta.15 to 3.12.0
- Rename package from number-to-bn to @metamask/number-to-bn

### Fixed
- Correctness bugfix: Update bn.js to fix hex encoding bug for certain large numbers
- Deprecate nodejs <8.17, npm<6

## [1.7.0]
### Changed
- Remove bad console log

## [1.6.0]
### Changed
- empty hex to zero
  - Empty hex 0x -> 0

## [1.5.0]
### Fixed
- Fixed hex number convetion, now if hex prefixed, always assumes base 16

## [1.4.0]
### Fixed
- Fix hex number shim

## [1.3.0]
### Added
- Added umd builds

### Changed
- better everythign
  - Better error messages
  - Far more comprehensive testing coverage
  - Far more support for hex string coverage
  - Far more support for number string coverage
  - Less lines of code, more bang for your buck
  - More config

## [1.2.0]
### Fixed
- decimal number fix
  - now throws under decimal number

## [1.1.0]
### Added
- es5 support

## [0.0.1]
### Added
- number-to-bn
  - Basic testing
  - Basic docs
  - License
  - basic exports

[Unreleased]: https://github.com/MetaMask/number-to-bn/compare/v1.7.1...HEAD
[1.7.1]: https://github.com/MetaMask/number-to-bn/compare/v1.7.0...v1.7.1
[1.7.0]: https://github.com/MetaMask/number-to-bn/compare/v1.6.0...v1.7.0
[1.6.0]: https://github.com/MetaMask/number-to-bn/compare/v1.5.0...v1.6.0
[1.5.0]: https://github.com/MetaMask/number-to-bn/compare/v1.4.0...v1.5.0
[1.4.0]: https://github.com/MetaMask/number-to-bn/compare/v1.3.0...v1.4.0
[1.3.0]: https://github.com/MetaMask/number-to-bn/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/MetaMask/number-to-bn/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/MetaMask/number-to-bn/compare/v0.0.1...v1.1.0
[0.0.1]: https://github.com/MetaMask/number-to-bn/releases/tag/v0.0.1
