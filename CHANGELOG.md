# Change Log
All notable changes to this project will be documented in this file. This change log follows the conventions of [keepachangelog.com](http://keepachangelog.com/).

<!-- (this space deliberately left blank) -->
<!-- ### Added -->
<!-- ### Changed -->
<!-- ### Removed -->
<!-- ### Fixed -->

## [Unreleased]
### Added
- `lambdaisland.uri.normalize/normalize`, for normalizing URI instances.

### Changed
- BREAKING: An empty path is now parsed as `""` instead of `nil`. This is per
  RFC3986: "A path is always defined for a URI, though the defined path may be
  empty (zero length).", it also mimics the behaviour of Addressable::URI.
- BREAKING: The port number is now parsed as a long/integer rather than a string.

## [1.1.0] - 2017-04-25
### Added
- Predicate functions `absolute?` and `relative?`

## 1.0.0 - 2017-02-23
### Added
- Initial release, public vars: `uri`, `join`, `coerce`, `parse`, `edn-readers`

[Unreleased]: https://github.com/lambdaisland/uri/compare/v1.1.0...HEAD
[1.1.0]: https://github.com/lambdaisland/uri/compare/v1.0.0...v1.1.0
