# iotprovision
iotprovision is a command-line utility for provisioning Microchip AVR-IoT, PIC-IoT and SAM-IoT kits for use with various cloud providers.

![PyPI - Format](https://img.shields.io/pypi/format/iotprovision)
![PyPI - Python Version](https://img.shields.io/pypi/pyversions/iotprovision)
![PyPI - License](https://img.shields.io/pypi/l/iotprovision)

## Overview
iotprovision is available:

* install using pip from pypi: https://pypi.org/project/iotprovision
* browse source code on github: https://github.com/microchip-pic-avr-tools/iotprovision
* read API documentation on github: https://microchip-pic-avr-tools.github.io/iotprovision
* read the changelog on github: https://github.com/microchip-pic-avr-tools/iotprovision/blob/main/CHANGELOG.md

## Command-line interface
Getting help:
```
iotprovision --help
```
The amount of logging is controlled by the -v/--verbose option:
```
iotprovision -v debug
```
Possible log levels are `debug`, `info`, `warning`, `error`, `critical`.  Default is `info`.

Print version info and exit:
```
iotprovision -V
```
Print release info and exit:
```
iotprovision -R
```
Provision for Amazon Web Services, using sandbox account:
```
iotprovision -c aws
```
Provision for Amazon Web Services, using MAR and custom account:
```
iotprovision -c aws -m mar
```
Provision for Amazon Web Services, using JITR and custom account:
```
iotprovision -c aws -m jitr
```
Provision for Google Cloud Platform:
```
iotprovision -c google
```
Provision for Azure:
```
iotprovision -c azure
```

## Notes for Linux® systems
This package uses pyedbglib and other libraries for USB transport and some udev rules are required.
For details see the pyedbglib package: https://pypi.org/project/pyedbglib
