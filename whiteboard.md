# Whiteboard

## Pre-config

### WiFi

On the boot volume, create `wpa_supplicant.conf` and add the following
(UPDATE DETAILS)

```
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
ap_scan=1
fast_reauth=1
country=JP

network={
	ssid="Your network's SSID"
	psk="Your network's password/psk"
	id_str="0"
	priority=100
}
```

### Enable SSH

add a blank text file named `ssh` in the boot volume