This folder contains tests based on Python unittest. Tests are run from the root of the repo (iot-provisioning-tool/ not iot-provisioning-tool/iotprovision or iot-provisioning-tool/ioiotprovision/tests)

To run all tests:
~~~~
\iot-provisioning-tool>python -m unittest discover
~~~~

To run a specific test module:
~~~~
\iot-provisioning-tool> python -m unittest iotprovision.tests.test_iotprovision_cli
~~~~

To run a specific test:
~~~~
\iot-provisioning-tool> python -m unittest iotprovision.tests.test_iotprovision_cli.TestIotprovisionCli.test_get_version
~~~~