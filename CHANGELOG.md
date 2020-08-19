# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [6.0.0-alpha.1] - 2020-08-19

### Added

- Full native TypeScript support.
- Nested "transactions" using `SAVEPOINT`.
- Native ECMAScript module support, including non-`default` exports for escaping and templating functions.
- A number of new APIs, including one for parsing a URL into configuration options, which can then be further customized.

### Changed

- Some configuration options may be slightly different if you use manual configuration.
- We now lint with `eslint`.
- We now format code with `prettier`'s default options.
- Much of the code has been heavily overhauled.
- Test coverage has been updated to 100% line coverage using `c8`.
- Escaping functions now always return `string` and never `number`.

### Fixed

- A few weird corner-cases should be better-defined, thanks to TypeScript.

### Removed

- Unfortunately, `cancel` support has been removed, because I couldn't find any documented way to support it. (And because Faraday no longer uses it anywhere.)