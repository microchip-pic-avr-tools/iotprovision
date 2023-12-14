[![MCHP](images/microchip.png)](https://www.microchip.com)

# iotprovision
iotprovision is a collection of applications or tools to support cloud provisioning of Microchip IoT boards.

Install using pip from [pypi](https://pypi.org/project/iotprovision):
```
pip install --user iotprovision
```

Browse source code on [github](https://github.com/microchip-pic-avr-tools/iotprovision)

Read API documentation on [github](https://microchip-pic-avr-tools.github.io/iotprovision)

Read the changelog on [github](https://github.com/microchip-pic-avr-tools/iotprovision/blob/main/CHANGELOG.md)

## Usage
iotprovision is used as a command-line interface

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
iotprovision --version
```
Print release info and exit:
```
iotprovision -R
```
Provision for Amazon Web Services, using Microchip sandbox account:
```
iotprovision -c aws
```
Provision for Amazon Web Services, using Multi-Account Registration (MAR) and custom account:
```
iotprovision -c aws -m mar
```
Provision for Amazon Web Services, using Just-In-Time Registration (JITR) and custom account:
```
iotprovision -c aws -m jitr
```
Provision for Azure:
```
iotprovision -c azure
```

## Certificate storage
Certificates and other files generated/retrieved during provisioning are stored in a hidden folder:

```
Windows:   C:\Users\<username>\.microchip-iot
Linux/Mac: $HOME/.microchip-iot
```

Files common for all kits are stored in the root of the folder, kit-specific files are stored
in subfolders identified with the kit serial number.


## Notes for Linux® systems
This package uses pyedbglib and other libraries for USB transport and some udev rules are required.
For details see the pyedbglib package: https://pypi.org/project/pyedbglib
