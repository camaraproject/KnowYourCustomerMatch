# Changelog KnowYourCustomerMatch

<!-- TOC:START -->
## Table of Contents
- [r2.1](#r21)
<!-- TOC:END -->

**Please be aware that the project will have frequent updates to the main branch. There are no compatibility guarantees associated with code in any branch, including main, until it has been released. For example, changes may be reverted before a release is published. For the best results, use the latest published release.**

The below sections record the changes for each API version in each release as follows:

* for an alpha release, the delta with respect to the previous release
* for the first release-candidate, all changes since the last public release
* for subsequent release-candidate(s), only the delta to the previous release-candidate
* for a public release, the consolidated changes since the previous public release

# r2.1

## Release Notes

This release candidate contains the definition and documentation of
* kyc-match 0.5.0-rc.1

The API definition(s) are based on
* Commonalities 0.8.0
* Identity and Consent Management 0.5.0

## kyc-match 0.5.0-rc.1

**kyc-match 0.5.0-rc.1 is a release-candidate version of this API.**

Changes documented below are compared to version 0.4.0.

- API definition **with inline documentation**:
  - [View it on ReDoc](https://redocly.github.io/redoc/?url=https://raw.githubusercontent.com/camaraproject/KnowYourCustomerMatch/r2.1/code/API_definitions/kyc-match.yaml&nocors)
  - [View it on Swagger Editor](https://camaraproject.github.io/swagger-ui/?url=https://raw.githubusercontent.com/camaraproject/KnowYourCustomerMatch/r2.1/code/API_definitions/kyc-match.yaml)
  - OpenAPI [YAML spec file](https://github.com/camaraproject/KnowYourCustomerMatch/blob/r2.1/code/API_definitions/kyc-match.yaml)

### Breaking changes

* Replace 403 INVALID_TOKEN_CONTEXT with 422 UNNECESSARY_IDENTIFIER by @GillesInnov35 in https://github.com/camaraproject/KnowYourCustomerMatch/pull/84
* Previously, when the API consumer provided both a 3-legged access token and an explicit `phoneNumber`, the API would return `403 INVALID_TOKEN_CONTEXT` if they did not match, but proceed as normal if they did match.
* Now, the API will always return `422 UNNECESSARY_IDENTIFIER` if both a 3-legged access token and an explicit `phoneNumber` are provided. This will be a breaking change for those API consumers who provide a matching 3-legged access token and `phoneNumber` - their API calls would have succeeded before, but now they will fail.

### Added

* Add bankaccountnumber as an attribute to KYC Match by @ToshiWakayama-KDDI in https://github.com/camaraproject/KnowYourCustomerMatch/pull/73

### Changed

* Alignment with Guidelines and linting rules for OWASP API Security  by @GillesInnov35 in https://github.com/camaraproject/KnowYourCustomerMatch/pull/72
* Commonalities 8.0.0 alignment and fix validation warnings by @GillesInnov35 in https://github.com/camaraproject/KnowYourCustomerMatch/pull/81
* Replace 403 INVALID_TOKEN_CONTEXT with 422 UNNECESSARY_IDENTIFIER by @GillesInnov35 in https://github.com/camaraproject/KnowYourCustomerMatch/pull/84
* Another update to fix validation warnings by @GillesInnov35 in https://github.com/camaraproject/KnowYourCustomerMatch/pull/83

### Fixed

* Correction of test definitions  by @GillesInnov35 in https://github.com/camaraproject/KnowYourCustomerMatch/pull/58

### Removed

* Remove idDocument related errors by @fernandopradocabrillo in https://github.com/camaraproject/KnowYourCustomerMatch/pull/54
* Remove Flows Image from yaml file by @GillesInnov35 in https://github.com/camaraproject/KnowYourCustomerMatch/pull/64

**Full Changelog**: https://github.com/camaraproject/KnowYourCustomerMatch/compare/r1.2...r2.1

