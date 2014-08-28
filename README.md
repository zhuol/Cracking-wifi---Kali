Cracking-wifi---Kali
====================

```
apt-get update
apt-get install linux-headers-$(uname -r)
apt-get apt-get update
apt-get install build-essential
apt-get install git
git clone https://github.com/lwfinger/rtl8188eu
cd rtl8188eu
make all
make install
insmod 8188eu.ko
 
ifconfig #(check to see if your wireless wlan cards is now listed)
 
#optional step ...reboot may be necessary
#sometimes a reboot helps pickup newly installed devices
reboot
```
