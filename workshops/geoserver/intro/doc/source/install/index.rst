.. _geoserver.install:

Installation
============

In this section we will setup the workshop virtual machine on your device.

GeoServer, being a Java application, typically requires a Java Runtime Environment (JRE) as well as an application server in order to function. The latest GeoServer version (2.10) requires a Java 8 JRE. Both of these are included with the virtual machine, so separate installation is not needed.

Setup
-----

This training course will use a virtual machine (VM) which has been already configured with GeoServer, eliminating the need to install it directly on your machine.

#. Install the latest version of VirtualBox (5.1.8) from the installer provided in the workshop package. You may keep all defaults during the install.

#. Double-click the VM image file that you downloaded or copied from the provided USB sticks (:file:`Geoserver_LT2016.ova`). This will import the virtual machine into VirtualBox.

#. Click :guilabel:`Import` to accept the defaults.

#. You will now see the :guilabel:`Geoserver_LT2016` entry in the list of virtual machines in VirtualBox.

.. note:: During install on Windows, you may see a warning about your network interfaces. **This is expected.** Your network connections will be *temporarily* disconnected, and automatically reset after installation has completed. So be aware that you don't want to be utilizing your network connection (for example, downloading something) during the installation of VirtualBox.


Starting and stopping services
------------------------------

The VM has been installed and when running GeoServer will be on by default. If GeoServer needs to be restarted, follow these steps:

#. Click the running VM to open the window. 

#. When prompted for :guilabel:`login` use **vagrant** and for :guilabel:`password` use **vagrant** as well.

#. The following command will start/stop/restart the GeoServer instance:

    .. code-block:: console
    
        sudo service geoserver restart