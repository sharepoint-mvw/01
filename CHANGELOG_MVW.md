## [5.03.04] - Unreleased

### Changed

- summary: Firmware Standardization: HMI Versioning
- details: Harmonized HMI firmware versioning to align with the standard vX.XX.XX format used by other boards

### Changed

- summary: Feature Update: USB Backup (Copy Function)
- details: Enhanced the COPY function to support USB backups and parameter comparison
- details: This feature becomes accessible via the HMI menu upon connecting a USB device. Inserting a USB drive automatically triggers a pop-up window with available options
- note: Note: Saving a backup to the USB drive does not require a password. However, restoring a backup from the USB drive to the inverter requires user login

### Added

- summary: Feature Update: CCE Board Temperature Monitoring
- details: Added parameter to display CCE board temperature, distinguishing it from AUI CPU temperature data

## [5.03.03] - 2026-01-14

### Added

- summary: New Protection: Electric Arc Detection (C7.17.1)
- details: Introduced configuration parameters for electric arc protection channels

## [5.03.02] - 2025-12-05

### Fixed

- summary: Bug Fix: HMI QR Code Redirect
- details: Resolved an issue where the QR code redirected to an incorrect product page

### Added

- summary: New Protection: Unconfigured CIB Interface (F0366)
- details: Added Fault F0366 to indicate communication between the CCE control board and an unconfigured CIB interface board

### Added

- summary: Feature Update: Load Parameter Set via Digital Input
- details: Enabled association of digital inputs to the "Load Parameter Set" function (C12.2, C12.3, C12.4)

### Deprecated

- summary: Deprecation: Grid Unbalance Fault (F2300)
- details: Deprecated F2300 (Grid Unbalance/Phase Loss). This protection is now covered by faults F0303, F0304, and F0305

### Added

- summary: Security Feature: Accessory Identification
- details: Implemented parameters to enforce identification of accessories in the AUI board expansion slot
- note: Note: Manual configuration is mandatory for cybersecurity compliance
- note: Note: A mismatch between configured and connected accessories will trigger an error

### Fixed

- summary: Bug Fix: Parameter Loading (F0100)
- details: Fixed a bug causing F0100 (Self-diagnosis failure) when loading default settings or parameter sets
- note: Note: In addition to the failure acting, changes will only take effect on the next startup

### Fixed

- summary: Bug Fix: HMI Parameter Search
- details: Resolved an issue preventing parameter editing when accessed via the HMI search function
- note: Note: This issue was isolated to the search function and did not affect menu navigation

### Fixed

- summary: DeviceNet Configuration Update
- details: Released EDS file v5.03.xx. Corrected the ProductCode (previously assigned to CFW900)
- note: Note: The previous code did not prevent operation but could cause network identification confusion

## [5.03.01] - 2025-10-16

### Added

- summary: Feature Update: Auxiliary Temperature Measurement
- details: Introduced auxiliary temperature measurement with support for feedback monitoring, alarms, and over-temperature protection
