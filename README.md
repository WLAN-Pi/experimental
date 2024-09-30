# Experimental

## hostapd eht and 6 GHz

Quick start:

```bash
wget https://github.com/WLAN-Pi/experimental/raw/main/hostapd_eht.zip
unzip hostapd_eht.zip
sudo ./hostapd 5ghz_eht.cfg
sudo ./hostapd 6ghz_eht.cfg
```

## wpa_supplicant with 802.11be support enabled

Quick start:
1. Add Wi-Fi 7 access point configuration to /etc/wpa_supplicant/wpa_supplicant.conf config file
2. Install 6.11 Linux kernel and experimental version of wpa_supplicant with 802.11be support enabled
```bash
wget https://github.com/WLAN-Pi/experimental/raw/main/wlanpi-kernel_1.20240916-1_arm64.deb.zip
unzip unzip wlanpi-kernel_1.20240916-1_arm64.deb.zip
sudo apt install ./wlanpi-kernel_1.20240916-1_arm64.deb
sudo reboot
wget https://github.com/WLAN-Pi/experimental/raw/main/wpa_supplicant_11be.zip
unzip wpa_supplicant_11be.zip
sudo ./wpa_supplicant -c /etc/wpa_supplicant/wpa_supplicant.conf -i wlan0
```
