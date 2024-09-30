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
2. Download experimental versio of wpa_supplicant which supports Wi-Fi 7
```bash
wget https://github.com/WLAN-Pi/experimental/raw/main/wpa_supplicant_11be.zip
unzip wpa_supplicant_11be.zip
sudo ./wpa_supplicant -c /etc/wpa_supplicant/wpa_supplicant.conf -i wlan0
```