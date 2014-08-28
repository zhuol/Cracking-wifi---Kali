Cracking-wifi---Kali
====================

<div style="width: 20%;">
    <img src="https://camo.githubusercontent.com/ac704739b3fad2580b44deeda8388c69edb98153/687474703a2f2f6272696c6c69616e746c79656173792e636f6d2f77702d636f6e74656e742f75706c6f6164732f323031342f30332f6c696e75785f746c2d776e3732356e2d686f77746f2e6a7067">
</div>

Install driver of Wireless Network Adapter on Kali Linux
---------------------
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
