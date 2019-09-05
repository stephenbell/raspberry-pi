## How to install Hass.io on an SD card

1. Download the [Hass.io](https://www.home-assistant.io/hassio/installation/) tarball
1. Flash the image onto an SD card using [Etcher](https://www.balena.io/etcher/)
1. Optional - set up the WiFi or static IP. There are two possible places for that: 
- On a blank USB stick with Fat32 partition (partition label: "CONFIG"), while in / directory, create `network/my-network` file 
- or on Hassio SD card first, bootable partition (might not be auto mounted in Linux) create `CONFIG/network/my-network` file 
For the content of this file follow the [HassOS howto][hassos-network].
