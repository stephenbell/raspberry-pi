## How to install Raspbian on an SD card

1. Download the [Raspbian](https://www.raspberrypi.org/downloads/) image
1. Flash the image onto an SD card using [Etcher](https://www.balena.io/etcher/)
1. Optional - enable SSH. While in / directory ("boot"), create empty file `ssh`
1. Optional - enable WiFi. While in / directory ("boot"), create file `wpa_supplicant.conf` with the following contents:
```css
country=US # Your 2-digit country code
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
network={
    ssid="YOUR_NETWORK_NAME"
    psk="YOUR_PASSWORD"
    key_mgmt=WPA-PSK
}
```
