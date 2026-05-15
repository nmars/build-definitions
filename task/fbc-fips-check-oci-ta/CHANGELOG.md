# Changelog

## Unreleased

### Fixed

- Updated the `fips-operator-check-step-action` revision parameter to use `check-payload` release `0.3.14`.

## 0.1

### Added

- Initial version of `fbc-fips-check-oci-ta` task
- Trusted Artifacts (`SOURCE_ARTIFACT`) variant of FBC fragment FIPS checking with `check-payload`
- Scans relatedImages from unreleased operator bundles in an FBC fragment image
- Parameters include `MAX_PARALLEL` and `image-mirror-set-path` for mirror resolution

### Note

This is the Trusted Artifacts variant of `fbc-fips-check` (`fbc-fips-check` uses a workspace source instead of `SOURCE_ARTIFACT`).
