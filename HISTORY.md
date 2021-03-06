# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.64.5] - 2020-11-25

### Fixed

- Fixed logic assigning output values to proxy classes after addon execution.

## [0.64.4] - 2020-10-26

### Changed

- Improved error messages logged when initializing a development session fails.

## [0.64.3] - 2020-10-21

### Fixed

- Fixed a case when tets name was not reported after session ends.
- Fixed IE driver re-initialization logic.

## [0.64.2] - 2020-10-13

### Fixed

- Fixed compatibility issue with ChromeOptions class, upgrading Guava library to version 29.
- Fixed a scenario in which instantiation of a proxy class failed during test name inferring.

## [0.64.1] - 2020-10-08

### Added 

- Added Generic driver to execute non-UI tests.

### Fixed

- Close the agent client when the driver quits to allow the process to exit.

## [0.64.0] - 2020-09-08

### Added 

- SDK will keep a development session open and only restart the driver when reporting the same Job (only when working with Agent 0.64.20 or newer).

## [0.63.5] - 2020-08-28

### Added 

- Screenshots are now being reported when command execution fails.
- Reporting extension for JUnit5 has been added.

### Fixed

- Removed bundled logback.xml that can interfere with explicitly specified logback configuration.

## [0.63.4] - 2020-08-07

### Fixed 

- Fixed false-failure happening when using Actions class and automatically reporting commands.

### Changed

- Now Driver and AgentClient will be closed gracefully when process terminates

### Added

- Added custom capability and documentation for execution using a cloud (e.g SauceLabs) driver.
- Junit4 Example

## [0.63.3] - 2020-07-15

### Fixed 

- Fixed reports not created when there is no package to infer a project name from.

## [0.63.2] - 2020-07-06

Initial release.
