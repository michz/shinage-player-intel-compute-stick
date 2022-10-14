# shinage-player-intel-compute-stick

Some candy for a Shinage Player on an Intel Compute Stick


## TODO

### debian installer bootstrap/automation/seeding

https://wiki.debian.org/DebianInstaller/Preseed

### WIFI

* activate non-free sources in sources.list
* apt install firmware-iwlwifi wpasupplicant
* Copy /etc/systemd/network/70-wlp1s0.network
* Copy /etc/systemd/system/wpa_supplicant@wlp1s0.service
* Copy and fill /etc/wpa_supplicant/wpa_supplicant-wlp1s0.conf
* `systemctl daemon-reload`
* `systemctl enable wpa_supplicant@wlp1s0.service`
* `systemctl enable systemd-networkd.service`
* Reboot
* Check status with `networkctl status wlp1s0`

### Filesystem optimizations

* Mount root volume with `noatime` and `data=writeback`
* Disable syslog (?)
* Disable systemd journal or disable writing of it to real disk

### Install


## TODO Candy

### EFI Boot Splash Image

