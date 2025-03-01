# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.X.X] - 2022-X-XX

## [1.3.7] - 2023-3-31
## Fixed
 - AUTOTOOL-3581: Data group load fails when cli preference list-all-properties is enabled

## [1.3.6] - 2022-12-9
## Changed
 - Update atg-shared-utilities to make use of primary admin user

## [1.3.5] - 2022-12-7
## Changed
 - Remove auth header when making requests to port 8100 with http. The request module will properly handle the default (which might not be admin)

## [1.3.4] - 2022-10-24
- More handling for race condition where updating data-group fails when it doesn't exist so it cannot be deleted

## [1.3.3] - 2022-5-5
## Changed
- Updated the release process documentation
- Fix race condition where updating data-group fails when it doesn't exist so it cannot be deleted

## [1.3.2] - 2022-3-18
## Changed
- Prevent persist from exiting early, when task is kicked off

## [1.3.1] - 2022-3-11
## Fixed
- StorageDataGroup: Speed up persist() by removing unused write cache logic

## [1.3.0] - 2022-1-18
## Changed
- Always save data to data group on write in StorageDataGroup

## [1.2.0] - 2022-1-7
## Added
- clearCache method
## Fixed
- Fix some security concerns with temporary file usage in StorageDataGroup

## [1.1.0] - 2021-5-6
## Added
- Add StorageJsonFile storage backend to persist on disk using JSON
## Fixed
- Fix collisions with multiple, concurrent data group writes

## [1.0.2] - 2020-12-21
### Fixed
- AUTOTOOL-2138: Data store initialization can fail from race condition

## [1.0.1] - 2020-12-18
### Changed
- AUTOTOOL-638: ([GitHub Issue 122](https://github.com/F5Networks/f5-appsvcs-extension/issues/122)) Data store interactions cause errors in mcpd log

## [1.0.0] - 2020-11-17
Initial release.
