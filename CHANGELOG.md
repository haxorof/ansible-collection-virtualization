# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased](../../releases/tag/X.Y.Z)

## [2.2.0](../../releases/tag/2.1.0) - 2025-10-04

## Added

- roles/docker_ce: Added support for Ubuntu 25 [@HRGCompany]

## Fixed

- roles/docker_ce: Docker removed nightly channel from repo-files
- roles/docker_ce: Failed to remove packages in Fedora when `docker_remove` and `docker_remove_all` are set to `true` due to package dependency.
- roles/docker_ce: software-properties-common not available on debian 13

## [2.1.0](../../releases/tag/2.1.0) - 2024-12-09

## Added

- roles/docker_ce: Support for DNF 5 in Fedora 41 and later [@wzzrd]
- roles/docker_ce: Added `docker_install_setup_repos_dependencies` for user to disable/enable any handing of dependencies related to repo setup.

## Changed

- roles/docker_ce: Improved handling between different package managers related to RedHat varity (e.g. yum, dnf, dnf5)

## Deprecated

- roles/docker_ce: Support for Python 2
- roles/docker_ce: Support for RHEL 7 and CentOS 7
- roles/docker_ce: Support for ansible-core 2.16
- roles/docker_ce: Linux Mint 18 and 19 in experimental variable `docker_x_mint_ubuntu_mapping`

## Fixed

- roles/docker_ce: Change repository URL for RHEL to use "rhel" instead of "centos"

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
