# Changelog

All notable changes to `laravel-permission-block` will be documented in this file

## 1.0.1 - 2023-07-14
### Changes
 - check blocked permission in `hasDirectPermission` method in `HasPermissions` trait
 - gates will check blocked permissions of user (only user, not role)

## 1.0.0 - 2023-06-30
### Added
 - function `hasBlockFromAnyPermission` to check any permissions array blocked for user
 - function `unblockFromPermission` to unblock permission

## 1.0.0-alpha - 2023-06-29
### Added

- function `blockFromPermission` to block user
- function `hasBlockFromPermission` to check permission is blocked for user
