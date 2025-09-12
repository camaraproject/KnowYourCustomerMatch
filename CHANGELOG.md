
# Changelog CAMARA KnowYourCustomer Match

## Table of Contents

- **[r1.2](#r12)**
- [r1.1](#r11)

**Please be aware that the project will have frequent updates to the main branch. There are no compatibility guarantees associated with code in any branch, including main, until it has been released. For example, changes may be reverted before a release is published. For the best results, use the latest published release.**

The below sections record the changes for each API version in each release as follows:

* for an alpha release, the delta with respect to the previous release
* for the first release-candidate, all changes since the last public release
* for subsequent release-candidate(s), only the delta to the previous release-candidate
* for a public release, the consolidated changes since the previous public release

**A previous changelog for this API can be found here: https://github.com/camaraproject/KnowYourCustomer/blob/main/CHANGELOG.md**

# r1.2

## Release Notes

This public release contains the definition and documentation of:
* know-your-customer-match v0.4.0 

The API definition(s) are based on
* Commonalities v0.6.0 [r3.3](https://github.com/camaraproject/Commonalities/releases/tag/r3.3)
* Identity and Consent Management v0.4.0 [r3.3](https://github.com/camaraproject/IdentityAndConsentManagement/releases/tag/r3.3)

## know-your-customer-match v0.4.0
This is the latest public release for the CAMARA KnowYourCustomer Match API, updating the previous release to the CAMARA Guidelines and Identity & Consent Management for the Meta Release Fall25. Some new input paramenters, to be matched, have been introduced.

- API definition **with inline documentation**:
  - OpenAPI [YAML spec file](https://github.com/camaraproject/KnowYourCustomerMatch/blob/r1.2/code/API_definitions/kyc-match.yaml)
  - [View it on ReDoc](https://redocly.github.io/redoc/?url=https://raw.githubusercontent.com/camaraproject/KnowYourCustomerMatch/r1.2/code/API_definitions/kyc-match.yaml&nocors)
  - [View it on Swagger Editor](https://camaraproject.github.io/swagger-ui/?url=https://raw.githubusercontent.com/camaraproject/KnowYourCustomerMatch/r1.2/code/API_definitions/kyc-match.yaml)

### Added
 * Support for the following use attributes to be matched: https://github.com/camaraproject/KnowYourCustomerMatch/pull/24
 * Undocumented Errors note in info.description: https://github.com/camaraproject/KnowYourCustomerMatch/pull/18
 
### Changed
 * Update x-correlator format: https://github.com/camaraproject/KnowYourCustomerMatch/pull/16

### Fixed
 * Fixed the missing externalDocs object and the order of two lines (version, commonalities version) by @ToshiWakayama-KDDI in PR#33 (M4 Release PR)  https://github.com/camaraproject/KnowYourCustomerMatch/pull/33
 * Fixed the new issues post M3 to meet M4 by @FabrizioMoggio in PR#28 (Wip for M4) https://github.com/camaraproject/KnowYourCustomerMatch/pull/28

### Removed
 * Removed AUTHENTICATION_REQUIRED error code: https://github.com/camaraproject/KnowYourCustomerMatch/pull/19
 * Removed wrong value in test plan by @fernandopradocabrillo in PR#26 https://github.com/camaraproject/KnowYourCustomerMatch/pull/26

**Full Changelog**: https://github.com/camaraproject/KnowYourCustomerMatch/commits/r1.1...r1.2



# r1.1

## Release Notes

This pre-release contains the definition and documentation of:
* know-your-customer-match v0.4.0-rc.1

The API definition(s) are based on
* Commonalities v0.6.0-rc.1
* Identity and Consent Management v0.4.0-rc.1

## know-your-customer-match v0.4.0-rc.1
This is the a release candidate for the CAMARA KnowYourCustomer Match API, updating the previous release to the CAMARA Guidelines and Identity & Consent Management for the Meta Release Fall25. Some new input paramenters, to be matched, have been introduced.

- API definition **with inline documentation**:
  - OpenAPI [YAML spec file](https://github.com/camaraproject/KnowYourCustomerMatch/blob/r1.1/code/API_definitions/kyc-match.yaml)
  - [View it on ReDoc](https://redocly.github.io/redoc/?url=https://raw.githubusercontent.com/camaraproject/KnowYourCustomerMatch/r1.1/code/API_definitions/kyc-match.yaml&nocors)
  - [View it on Swagger Editor](https://camaraproject.github.io/swagger-ui/?url=https://raw.githubusercontent.com/camaraproject/KnowYourCustomerMatch/r1.1/code/API_definitions/kyc-match.yaml)

## Please note:

- This pre-release contains a release-candidate API version, there are bug fixes to be expected and incompatible changes in upcoming versions 
- The release is suitable for implementers, but it is not recommended to use the API with customers in productive environments
- The release scope is defined here: https://github.com/camaraproject/KnowYourCustomerMatch/issues/22

### Added
 * Support for the following use attributes to be matched: https://github.com/camaraproject/KnowYourCustomerMatch/pull/24
 * Undocumented Errors note in info.description: https://github.com/camaraproject/KnowYourCustomerMatch/pull/18
 
### Changed
 * Update x-correlator format: https://github.com/camaraproject/KnowYourCustomerMatch/pull/16

### Fixed

### Removed
 * Removed AUTHENTICATION_REQUIRED error code: https://github.com/camaraproject/KnowYourCustomerMatch/pull/19

## New Contributors
* @FabrizioMoggio

**Full Changelog**: https://github.com/camaraproject/KnowYourCustomerMatch/commits/r1.1
