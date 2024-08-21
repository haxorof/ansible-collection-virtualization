# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased](../../releases/tag/X.Y.Z)

## [2.0.0](../../releases/tag/2.0.0) - 2024-08-21

## Added

- roles/docker_ce: Added support for Amazon Linux
- roles/docker_ce: Added support to bypass package manager GPG key verification
- roles/docker_ce: Added Linux Mint 22 mapping

## Removed

- roles/docker_ce: Removed support for devicemapper since it was removed from Docker Engine v25.
- roles/docker_ce: Removed support to install Docker Compose via Pip.
- roles/docker_ce: Remove tasks which uninstalls Docker versions before Docker CE
- roles/docker_ce: Removed handling of old Ubuntu and Debian systems systems without SNI
- roles/docker_ce: Removed tasks to handle older Docker CE versions 17 and 18
- roles/docker_ce: Removed task related to compatibility for no longer officially supported distributions since Docker CE 18.09

## [1.1.0](../../releases/tag/1.1.0) - 2024-03-08

## Added

- Added support for ARM64 in docker_ce role.

## [1.0.0](../../releases/tag/1.0.0) - 2023-12-09

### Added

- Added role docker_ce, same as Ansible standalone role haxorof.docker_ce
