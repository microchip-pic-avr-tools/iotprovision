iotprovision package
====================

Subpackages
-----------

.. toctree::
   :maxdepth: 4

   iotprovision.aws
   iotprovision.azure
   iotprovision.cellular
   iotprovision.winc

Submodules
----------

Provisioning main()
-------------------

.. automodule:: iotprovision.iotprovision
   :undoc-members:
   :show-inheritance:

Provisioning
------------

.. automodule:: iotprovision.provisioner
   :members:
   :undoc-members:
   :show-inheritance:

Firmware interface
------------------

.. automodule:: iotprovision.firmwareinterface
   :members:
   :undoc-members:
   :show-inheritance:

ECC storage
-----------

.. automodule:: iotprovision.eccstorage
   :members:
   :undoc-members:
   :show-inheritance:

Kit reconfiguration
-------------------

.. automodule:: iotprovision.kit_config
   :members:
   :undoc-members:
   :show-inheritance:

Global configuration
--------------------
   
.. autoclass:: iotprovision.config.Config
   :noindex:

   .. autoclass:: iotprovision.config.Config.Certs
      :exclude-members: certs_dir
      :members:
      :undoc-members:
      :show-inheritance:
      :noindex:

      .. autoattribute:: iotprovision.config.Config.Certs.certs_dir
         :annotation: $home/.microchip-iot
   
Module contents
---------------

.. automodule:: iotprovision
   :members:
   :undoc-members:
   :show-inheritance:
