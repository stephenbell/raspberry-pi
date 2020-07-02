====================================
How to install Hass.io on an SD card
====================================

#. Download the Hass.io_ tarball 

#. Flash the image onto an SD card using a tool such as balenaEtcher_

Optional - set up the Wi-Fi or a static IP address. There are two possible places for that:

- On a blank USB stick with a FAT32 partition having partition label CONFIG, while in its root directory, create the network/my-network file, or
- On the Home Assistant SD card’s first, bootable partition (labeled hassos-boot, might not be auto mounted in Linux) create the CONFIG/network/my-network file.

For the content of this file, follow the Home Assistant Operating System howto_.

.. _Hass.io: https://www.home-assistant.io/hassio/installation/
.. _balenaEtcher: https://www.balena.io/etcher/
.. _howto: https://github.com/home-assistant/operating-system/blob/dev/Documentation/network.md