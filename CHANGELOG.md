# Changelog

## [2.10.6] - October 2022

### Changed
- DSG-5161 Moved device certificate and private key from slot 0 to slot 18 to conform with Sequans requirements (Sequans FW >= 8.0.5.11)
- DSG-5563 Added notification if Sequans firmware is out of date
- DSG-5008 Switch to using ATdriver from pysequansutils
- DSG-5078 Updated bundled debugger firmware (1.25.116)
- DSG-5458 Added metadata tag for Python 3.10
- DSG-5546 Removed metadata tag for Python 3.6
- DSG-5614 Updated pykitcommander dependency requirement (to use updated provisioning firmware)
- DSG-5618 Improved error reporting for serial port detection
- DSG-5624 Updated pyedbglib dependency requirement for improved serial port detection
- DSG-5628 Changed behaviour of -P switch to override an automatically detected port; Changed -p to -P in pywinc utility.

## [2.8.5] - June 2022

### Added
- DSG-4600 Support for SAM-IoT provisioning
- DSG-4818 Support for AVR-IoT Cellular Mini provisioning

### Changed
- DSG-4868 Removed full stack trace when using info logging
- DSG-5013 Added Amazon root CA bundle as recommended by Amazon (pyawsutils dependency)
- DSG-4214, DSG-4198, DSG-4185, DSG-4360 Provisioning output cosmetic improvements
- DSG-4323, DSG-4297 Debugger firmware upgrade not mandatory after v1.15
- DSG-3019, DSG-3017, DSG-3346, DSG-4188, DSG-4869 improvements to WINC handling

## [2.5.21] - December 2021

### Added
- DSG-3048 Added option to skip programming provisioning firmware
- DSG-3049 Added certificate blob build and upload (pywinc)
- DSG-3804 Python 3.9 support
- DSG-4175 Temporary click-me link for Azure

### Fixed
- DSG-4232, DSG-4330 Improved target firmware interaction stability
- DSG-3491 iotprovision (MAR) incorrect warning on default organization name

### Changed
- DSG-4198, DSG-4214, DSG-4295, DSG-2999 Improved output
- DSG-4323 Only upgrade debugger if version is lower than 1.15.479
- DSG-3015 Update pywinc CLI to use pykitcommander
- DSG-3070 No AWS account settings are altered
- DSG-3140 Prevent auto-amazon of iotprovisioning
- DSG-3393 Moved provisioning logic from pyazureutils to iotprovision
- DSG-4177 Bundle latest released nEDBG/PKOB nano FW (1.22.73)
- DSG-3141 Improve novice users CLI experience

## [2.1.2] - February 2021
- First public release to PyPi
