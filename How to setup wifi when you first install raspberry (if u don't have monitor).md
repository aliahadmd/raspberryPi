How to setup wifi when you first install raspberry (if u don't have monitor) :
------------------------------------------------------------------------------
1. go to windows machine 
2. go to ssd folder
3. inside folder create a new file to configure wifi
4. name it " wpa_supplicant.conf "
5.open file with any text editor.
6. write it:
```
country=US
ctrl_interface=DIR=/var/run/wpa_supplicant Group=netdev
update_config=1

network={
scan_ssid=1
ssid="your_wifi_ssid"
psk="your_wifi_password"
}
```
