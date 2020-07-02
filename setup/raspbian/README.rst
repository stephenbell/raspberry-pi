=====================================
How to install Raspbian on an SD card
=====================================

#. Download the Raspbian_ image.

#. Flash the image onto an SD card using a tool such as balenaEtcher_.

Optional -

#. To enable SSH, place a file named ssh, without any extension, in the boot folder on the SD card.

#. To enable WiFi, you will need to define a wpa_supplicant.conf file for your particular wireless network. Put this file in the boot folder, and when the Pi first boots, it will copy that file into the correct location in the Linux root file system and use those settings to start up wireless networking.

   wpa_supplicant.conf file example:

   .. code-block:: bash

      country=US
      ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
      update_config=1

      network={
         ssid="<Name of your wireless LAN>"
         psk="<Password hash for your wireless LAN>"
      }
   
   .. note:: The "password hash" can be generated using wpa_passphrase on the command line.

.. _Raspbian: https://www.raspberrypi.org/downloads/
.. _balenaEtcher: https://www.balena.io/etcher/
