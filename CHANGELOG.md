# Change Log

[Releases](https://github.com/NetApp/netappdvp/releases)

## Changes since 1.4.0

**Fixes:**

- Stopped using redundant debug parameter from config file.
- Prevent creating volumes with duplicate names on SolidFire.
- Fixed cloning from a snapshot in SolidFire.
- Fixed a rare SliceNotRegistered error when cloning volumes with SolidFire.
- Resolved an iSCSI attachment bug when using multipathing.

**Enhancements:**

- Added release notes (CHANGELOG.md).
- Added minimum ONTAP version check.
- Logging enhancements: log rotation, log level control, simultaneous logging
to console and file.
- Added default ONTAP volume creation options to config.json that were previously only available via '-o'.
- Added ONTAP securityStyle option handling.
- Added default volume size to config file.
- Standardized volume size format across ONTAP, SolidFire, and E-series drivers.
- Reduced log spam when debug logging is enabled with SolidFire.
- Moved README.md contents to [Read the Docs](http://netappdvp.readthedocs.io/en/latest/).
- `.snapshots` directory is now hidden in ONTAP NFS mounts by default.
