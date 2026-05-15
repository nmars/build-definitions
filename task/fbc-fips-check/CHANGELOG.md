# Changelog

## Unreleased

### Fixed

- Updated the `fips-operator-check-step-action` revision parameter to use `check-payload` release `0.3.14`.

## 0.1

### Added

- Initial version of `fbc-fips-check` task
- FBC fragment FIPS checking with `check-payload` for unreleased operator bundles
- Legacy bundle exemption for qualifying Red Hat subscriptions when the bundle predates the FIPS requirement date (January 31, 2025), unless the bundle explicitly claims FIPS compliance
- Parameters include `MAX_PARALLEL` and `image-mirror-set-path` for mirror resolution

### Note

Workspace-source variant; the Trusted Artifacts equivalent is `fbc-fips-check-oci-ta`.
