# Realtek rtl8188e Linux Drivers (v5.2.2.4)

## Supports
* rtl8188eus | rtl8188eu | rtl8188etv Chipsets.
* Up to Linux Kernel v5.8+

# Howto build and install :
1. Install required tools and clone this repositor :
```
$ sudo apt-get install gcc
$ git clone https://github.com/pkm774/RTL8188E_DRIVERS rtl8188e
```
2. Enter in cloned directory and start building :
```
$ cd rtl8188e
$ make
```
3. Install wlan driver module (as sudo user only):
```
$ sudo make install
```
4. Restart Network Manager :
```
$ sudo systemctl restart NetworkManager
```
5. If driver is still not working, Reboot your System.
6. Done !

# Load/Unload Module Directly :
1. Follow above method upto 2nd Step.
2. Load compiled module directly using insmod :
```
$ sudo insmod 8188eu.ko
```
3. Done !, Adapter will start working.
4. For unloading Module type :
```
$ sudo rmmod 8188eu
```

### Driver can be modified according to user through Makefile.

# Driver Credits
Realtek       - https://www.realtek.com<br>
aircrack-ng.  - https://www.aircrack-ng.org<br>
<br>All Contributers and Users<br>
