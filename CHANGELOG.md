# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),

## [Unreleased] - XX-XX-XX

### Added

- Ubuntu 19.04 (disco) support

### Changed

- Improve code quality according to codacy checkup

# [3.6.2] - 2019-04-24

### Added

- Additional GCC flags : "-Wno-error=date-time for Debian" : PR [#52](https://github.com/VirtuBox/nginx-ee/pull/52)

### Changed

- Update LibreSSL to v2.9.1
- Update Nginx stable to 1.16.0

## [3.6.1] - 2019-04-19

### Added

- Latest Pcre version auto-update

### Fixed

- OpenSSL selection from script arguments
- Pcre library update

## [3.6.0] - 2019-04-18

### Added

- LibreSSL support with the flag --libressl
- OpenSSL release choice : 1.1.1b by default, or 3.0.0-dev or system lib

### Changed

- Improve Nginx setup from scratch
- Update openssl-patch
- Nginx is compiled with OpenSSL 1.1.1b stable by default
- Update PCRE LIB to v8.43

### Fixed

- RTMP variable check
- Nginx package hold with WordOps

## [3.5.2] - 2019-02-18

### Changed

- fix debian 8 build
- fix dynamic modules choice

## [3.5.1] - 2019-02-07

### Changed

- improve openssl download and patching
- improve code quality
- improve travis build configuration
- update repository image

### Added

- add infos about auto-update cronjob
- Add support for Raspbian Stretch
- Add Cloudflare zlib
- Add dynamic module compilation in interactive installation menu
- Add cronjob setup in interactive installation menu

## [3.5.0] - 2018-12-26

### Changed

- uwsgi support re-added
- set back apt-mark hold on sw-nginx package for Plesk

### Added

- added daily cronjob for automated update
- Add support for Debian 9 & Raspbian

## [3.4.0] - 2018-12-26

### Changed

- Fix gcc setup with nginx stable release
- Fix arguments parsing for non-interactive install
- By default Nginx-ee compile the latest mainline release without optional modules like pagespeed or naxsi
- Fix wrong Nginx version displayed in the compilation summary

### Added

- Interactive install can be launched with the argument -i or --interactive
- Add WordOps detection

## [3.3.3] - 2018-12-07

### Changed

- Fix RTMP module choice by @Madic- [Pull request #23](https://github.com/VirtuBox/nginx-ee/pull/23)
- Update openssl-patch url

## [3.3.2] - 2018-11-27

### Added

- Add changelog
- add compilation summary

### Changed

- fix nginx compilation arguments
- cleanup code
- openssl version bump to 1.1.2-dev

## [3.3.1] - 2018-11-16

### Changed

- fix nginx version detection
- cleanup code
- update github page

## [3.3.0] - 2018-11-15

### Changed

- Add the ability to override official & third-party modules built with nginx-ee
- Automate nginx release number detection for mainline and stable release
- Do not lock nginx packages updates with apt-mark anymore but directly with /etc/apt/preferences.d/