# Xunison-Exigo-Hub-D50-5G
My OpenWrt SNAPSHOT / LuCI Main build for the Xunison Exigo Hub D50 5G router [Build: 24.05.2026].

<p align="center">
<img src="https://github.com/4IceG/Personal_data/blob/master/xunisondevb.png?raw=true" />
</p>

![GitHub release (latest by date)](https://img.shields.io/github/v/release/4IceG/Xunison-Exigo-Hub-D50-5G?style=flat-square)
![GitHub stars](https://img.shields.io/github/stars/4IceG/Xunison-Exigo-Hub-D50-5G?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/4IceG/Xunison-Exigo-Hub-D50-5G?style=flat-square)
![GitHub All Releases](https://img.shields.io/github/downloads/4IceG/Xunison-Exigo-Hub-D50-5G/total)

### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> Languages available / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Dostępne języki

<img src="https://hatscripts.github.io/circle-flags/flags/cz.svg" width="48" title="Czech (Čeština)" alt="Czech language" /> <img src="https://hatscripts.github.io/circle-flags/flags/dk.svg" width="48" title="Danish (Dansk)" alt="Danish language" /> <img src="https://hatscripts.github.io/circle-flags/flags/de.svg" width="48" title="German (Deutsch)" alt="German language" /> 
<img src="https://hatscripts.github.io/circle-flags/flags/es.svg" width="48" title="Spanish (Español)" alt="Spanish language" /> <img src="https://hatscripts.github.io/circle-flags/flags/fr.svg" width="48" title="French (Français)" alt="French language" /><img src="https://hatscripts.github.io/circle-flags/flags/it.svg" width="48" title="Italian (Italiano)" alt="Italian language" /> 
<img src="https://hatscripts.github.io/circle-flags/flags/jp.svg" width="48" title="Japanese (日本語)" alt="Japanese language" /> <img src="https://hatscripts.github.io/circle-flags/flags/kr.svg" width="48" title="Korean (한국어)" alt="Korean language" /><img src="https://hatscripts.github.io/circle-flags/flags/nl.svg" width="48" title="Dutch (Nederlands)" alt="Dutch language" /> 
<img src="https://hatscripts.github.io/circle-flags/flags/pl.svg" width="48" title="Polish (Polski)" alt="Polish language" /> <img src="https://hatscripts.github.io/circle-flags/flags/br.svg" width="48" title="Brazilian Portuguese (Português Brasil)" alt="Brazilian Portuguese language" /> <img src="https://hatscripts.github.io/circle-flags/flags/ru.svg" width="48" title="Russian (Русский)" alt="Russian language" /> <img src="https://hatscripts.github.io/circle-flags/flags/vn.svg" width="48" title="Vietnamese (Tiếng Việt)" alt="Vietnamese language" /> <img src="https://hatscripts.github.io/circle-flags/flags/cn.svg" width="48" title="Simplified Chinese (简体中文)" alt="Simplified Chinese language" /> <img src="https://hatscripts.github.io/circle-flags/flags/tw.svg" width="48" title="Traditional Chinese (繁體中文 - 台灣)" alt="Traditional Chinese language" /> <img src="https://hatscripts.github.io/circle-flags/flags/hk.svg" width="48" title="Traditional Chinese (繁體中文 - 香港)" alt="Traditional Chinese language" />

### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> OpenWrt installation procedure / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Procedura instalacji OpenWrt

<details>
   <summary>Pokaż | Show me</summary>

![](https://forum.openwrt.org/uploads/default/original/3X/d/9/d92a1660e463e3b93a9c53158456a9fa1b3599ce.png)

Installing firmware / Recovery steps
1. Turn off the power
2. Press and hold the reset button
3. Turn on the power (reset cannot be released, the internet light will stay on after 10s)
4. Set the computer IP address to 192.168.1.2
subnet mask 255.255.255.0
gateway 192.168.1.1
5. Open the computer browser and enter 192.168.1.254
6. Select the firmware file (factory)
7. Click the update button once and wait for the router to restart
  
</details>

### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> What You Should Know / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Co powinieneś wiedzieć

+ #### Installation of additional packages / Instalacja dodatkowych pakietów
> Snapshots are built daily, and that sets time limits to installing new packages with apk. Due to kernel version checksums, you can only install “kmod” kernel modules and other kernel version dependent modules from the exactly same snapshot build. So, a few hours after flashing the firmware you may not be able to install new modules with opkg any more (as the next snapshot has been built into the download repo and has different checksums).   
> Obrazy snapshots budowane są codziennie, a to ustawia limity czasowe na instalację nowych pakietów za pomocą apk. Z powodu sum kontrolnych wersji jądra, możesz zainstalować tylko moduły "kmod" i inne moduły zależne od wersji jądra z dokładnie tego samego snapshotu. Tak więc, kilka godzin po flashowaniu firmware możesz nie być w stanie zainstalować nowych modułów za pomocą opkg (ponieważ następny snapshot został wbudowany w repo i ma inne sumy kontrolne).

+ #### User's own configuration / Konfiguracja przez użytkownika
> The user must configure on his own:
- interface for modem (Quectel >> requires APN settings and checked option "Bring up on boot")
- set up Wi-Fi/passwords
> Użytkownik musi skonfigurować we własnym zakresie:
- interfejs dla modemu (Quectel >> wymaga ustawienia apn i zaznaczenia opcji autostartu połączenia)
- skonfigurować Wi-Fi/hasła

+ #### LuCI theme / Motyw LuCI
> Main theme: Bootstrap.   
> Główny motyw: Bootstrap.

+ #### My modifications / Moje modyfikacje
> I installed the [luci-app-exigo-hub-d50-5g](https://github.com/4IceG/luci-app-exigo-hub-d50-5g/tree/main) package (it configures router and my packages, controls 4G and 5G LEDs).   
> Dodałem pakiet [luci-app-exigo-hub-d50-5g](https://github.com/4IceG/luci-app-exigo-hub-d50-5g/tree/main) (wstępnie ustawia router i moje pakiety, steruje LED-ami 4G i 5G).

+ #### Modem requires following packages to work in pcie mode / Modem do działania w pcie wymaga pakietów
> [Quectel-wwan-mini](https://github.com/4IceG/Quectel-wwan-mini) (mhi_q & quectel-cm & luci-proto-quectel) + [luci-app-exigo-hub-d50-5g](https://github.com/4IceG/luci-app-exigo-hub-d50-5g)

### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> Screenshot / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Zrzut ekranu

![](https://github.com/4IceG/Personal_data/blob/master/5G/Xunison.png?raw=true)

### Packages available in the image / Pakiety dostępne w obrazie:
<details>
   <summary>Pokaż | Show me</summary>
   
``` bash
apk-mbedtls
ath11k-firmware-ipq5018
ath11k-firmware-qcn9074
atinout
base-files
bc
block-mount
busybox
ca-bundle
ca-certificates
cgi-io
chat
comgt
coreutils
coreutils-stat
curl
dbus
debugfs
dnsmasq
dropbear
e2fsprogs
ekoonepl-luci
ekooneplstat
ekooneplusb
ekooneplusb-luci
ethtool-full
f2fsck
firewall4
fstools
fwtool
getrandom
glib2
glib2-core
glib2-gio
glib2-gmodule
glib2-gobject
glib2-gthread
hostapd-common
ip-tiny
ipq-wifi-xunison_exigo-hub-d50-5g
iw
jansson4
jshn
jsonfilter
kernel
kmod-ath
kmod-ath11k
kmod-ath11k-ahb
kmod-ath11k-pci
kmod-button-hotplug
kmod-cfg80211
kmod-crypto-aead
kmod-crypto-cbc
kmod-crypto-ccm
kmod-crypto-cmac
kmod-crypto-crc32
kmod-crypto-crc32c
kmod-crypto-ctr
kmod-crypto-des
kmod-crypto-ecb
kmod-crypto-gcm
kmod-crypto-geniv
kmod-crypto-gf128
kmod-crypto-ghash
kmod-crypto-hash
kmod-crypto-hmac
kmod-crypto-kpp
kmod-crypto-lib-chacha20
kmod-crypto-lib-chacha20poly1305
kmod-crypto-lib-curve25519
kmod-crypto-lib-poly1305
kmod-crypto-manager
kmod-crypto-md5
kmod-crypto-michael-mic
kmod-crypto-null
kmod-crypto-rng
kmod-crypto-seqiv
kmod-crypto-sha1
kmod-crypto-sha256
kmod-crypto-sha3
kmod-crypto-sha512
kmod-dsa
kmod-dsa-qca8k
kmod-dsa-realtek
kmod-fixed-phy
kmod-fs-exfat
kmod-fs-ext4
kmod-fs-f2fs
kmod-fs-netfs
kmod-fs-ntfs3
kmod-fs-vfat
kmod-gpio-button-hotplug
kmod-hwmon-core
kmod-i2c-core
kmod-i2c-mux
kmod-i2c-mux-pinctrl
kmod-input-core
kmod-input-leds
kmod-keys-encrypted
kmod-keys-trusted
kmod-leds-gpio
kmod-leds-pwm
kmod-ledtrig-activity
kmod-ledtrig-gpio
kmod-ledtrig-network
kmod-ledtrig-pattern
kmod-lib-crc-ccitt
kmod-lib-crc16
kmod-lib-crc32c
kmod-libphy
kmod-mac80211
kmod-mdio-devres
kmod-mhi-bus
kmod-mhi-net
kmod-mii
kmod-mmc
kmod-mux-core
kmod-mux-gpio
kmod-net-selftests
kmod-nf-conntrack
kmod-nf-flow
kmod-nf-log
kmod-nf-log6
kmod-nf-nat
kmod-nf-reject
kmod-nf-reject6
kmod-nfnetlink
kmod-nfnetlink-queue
kmod-nft-core
kmod-nft-fib
kmod-nft-nat
kmod-nft-offload
kmod-nft-queue
kmod-nls-base
kmod-nls-cp437
kmod-nls-iso8859-1
kmod-nls-utf8
kmod-oid-registry
kmod-pcie_mhi
kmod-phy-at803x
kmod-phy-qca83xx
kmod-phy-realtek
kmod-phy-rtl8261n
kmod-phy-smsc
kmod-phylib-qcom
kmod-phylink
kmod-ppp
kmod-pppoe
kmod-pppox
kmod-qca-nss-dp
kmod-qca-ssdk
kmod-qcom-qmi-helpers
kmod-qrtr
kmod-qrtr-mhi
kmod-qrtr-smd
kmod-r8125
kmod-r8126
kmod-r8127
kmod-r8169
kmod-random-core
kmod-regmap-core
kmod-scsi-core
kmod-slhc
kmod-thermal
kmod-tpm
kmod-udptunnel4
kmod-udptunnel6
kmod-usb-acm
kmod-usb-common
kmod-usb-core
kmod-usb-dwc2
kmod-usb-dwc2-pci
kmod-usb-dwc3
kmod-usb-dwc3-qcom
kmod-usb-ehci
kmod-usb-ledtrig-usbport
kmod-usb-net
kmod-usb-net-cdc-ether
kmod-usb-net-cdc-mbim
kmod-usb-net-cdc-ncm
kmod-usb-net-huawei-cdc-ncm
kmod-usb-net-qmi-wwan
kmod-usb-ohci
kmod-usb-phy-nop
kmod-usb-roles
kmod-usb-serial
kmod-usb-serial-ch341
kmod-usb-serial-option
kmod-usb-serial-qualcomm
kmod-usb-serial-wwan
kmod-usb-storage
kmod-usb-storage-uas
kmod-usb-uhci
kmod-usb-wdm
kmod-usb-xhci-hcd
kmod-usb2
kmod-usb2-pci
kmod-usb3
kmod-usbmon
kmod-wireguard
kmod-wwan
libatomic1
libattr
libblkid1
libblobmsg-json20260313
libc
libcomerr0
libcurl4
libdbus
libe2p2
libevdev
libexpat
libext2fs2
libf2fs6
libffi
libgcc1
libgpiod
libiwinfo-data
libiwinfo20230701
libjson-c5
libjson-script20260313
libkmod
liblua5.1.5
liblucihttp-lua
liblucihttp-ucode
liblucihttp0
libmbedtls21
libmbim
libmnl0
libncurses6
libnftnl11
libnghttp2-14
libnl-core200
libnl-genl200
libnl-tiny1
libpci
libpcre2
libpthread
libqmi
libqrtr-glib
libreadline8
librt
libsensors5
libsmartcols1
libss2
libsysfs2
libubox20260313
libubus-lua
libubus20251202
libuci20250120
libuclient20201210
libucode20230711
libudebug
libudev-zero
libusb-1.0-0
libustream-mbedtls20201210
libuuid1
logd
losetup
lua
luci
luci-app-atinout
luci-app-backupandrestore-apk
luci-app-commands
luci-app-cpu-perf
luci-app-cpu-status
luci-app-crontab-wizard
luci-app-easyconfig-transfer
luci-app-ekooneplstat
luci-app-exigo-hub-d50-5g
luci-app-filemanager
luci-app-firewall
luci-app-internet-detector
luci-app-ledtrig-rssi
luci-app-ledtrig-switch
luci-app-ledtrig-usbport
luci-app-lite-watchdog
luci-app-modemband
luci-app-modemdata
luci-app-package-manager
luci-app-ports-status-mod
luci-app-qfirehose
luci-app-sms-tool-js
luci-app-used-channels
luci-app-wifihistory
luci-base
luci-compat
luci-i18n-atinout-de
luci-i18n-atinout-es
luci-i18n-atinout-fr
luci-i18n-atinout-it
luci-i18n-atinout-pl
luci-i18n-atinout-ru
luci-i18n-atinout-vi
luci-i18n-atinout-zh-cn
luci-i18n-atinout-zh-tw
luci-i18n-backupandrestore-apk-de
luci-i18n-backupandrestore-apk-es
luci-i18n-backupandrestore-apk-fr
luci-i18n-backupandrestore-apk-it
luci-i18n-backupandrestore-apk-pl
luci-i18n-backupandrestore-apk-ru
luci-i18n-backupandrestore-apk-vi
luci-i18n-backupandrestore-apk-zh-cn
luci-i18n-backupandrestore-apk-zh-tw
luci-i18n-base-de
luci-i18n-base-es
luci-i18n-base-fil
luci-i18n-base-fr
luci-i18n-base-it
luci-i18n-base-pl
luci-i18n-base-ru
luci-i18n-base-vi
luci-i18n-base-zh-cn
luci-i18n-base-zh-tw
luci-i18n-commands-de
luci-i18n-commands-es
luci-i18n-commands-fr
luci-i18n-commands-it
luci-i18n-commands-pl
luci-i18n-commands-ru
luci-i18n-commands-vi
luci-i18n-commands-zh-cn
luci-i18n-commands-zh-tw
luci-i18n-cpu-perf-de
luci-i18n-cpu-perf-es
luci-i18n-cpu-perf-fr
luci-i18n-cpu-perf-it
luci-i18n-cpu-perf-pl
luci-i18n-cpu-perf-ru
luci-i18n-cpu-perf-vi
luci-i18n-cpu-perf-zh-cn
luci-i18n-cpu-perf-zh-tw
luci-i18n-cpu-status-de
luci-i18n-cpu-status-es
luci-i18n-cpu-status-fr
luci-i18n-cpu-status-it
luci-i18n-cpu-status-pl
luci-i18n-cpu-status-ru
luci-i18n-cpu-status-vi
luci-i18n-cpu-status-zh-cn
luci-i18n-cpu-status-zh-tw
luci-i18n-crontab-wizard-de
luci-i18n-crontab-wizard-es
luci-i18n-crontab-wizard-fr
luci-i18n-crontab-wizard-it
luci-i18n-crontab-wizard-pl
luci-i18n-crontab-wizard-ru
luci-i18n-crontab-wizard-vi
luci-i18n-crontab-wizard-zh-cn
luci-i18n-crontab-wizard-zh-tw
luci-i18n-easyconfig-transfer-de
luci-i18n-easyconfig-transfer-es
luci-i18n-easyconfig-transfer-fr
luci-i18n-easyconfig-transfer-it
luci-i18n-easyconfig-transfer-pl
luci-i18n-easyconfig-transfer-ru
luci-i18n-easyconfig-transfer-vi
luci-i18n-easyconfig-transfer-zh-cn
luci-i18n-easyconfig-transfer-zh-tw
luci-i18n-ekooneplstat-de
luci-i18n-ekooneplstat-es
luci-i18n-ekooneplstat-fr
luci-i18n-ekooneplstat-it
luci-i18n-ekooneplstat-pl
luci-i18n-ekooneplstat-ru
luci-i18n-ekooneplstat-vi
luci-i18n-ekooneplstat-zh-cn
luci-i18n-ekooneplstat-zh-tw
luci-i18n-exigo-hub-d50-5g-de
luci-i18n-exigo-hub-d50-5g-es
luci-i18n-exigo-hub-d50-5g-fr
luci-i18n-exigo-hub-d50-5g-it
luci-i18n-exigo-hub-d50-5g-pl
luci-i18n-exigo-hub-d50-5g-ru
luci-i18n-exigo-hub-d50-5g-vi
luci-i18n-exigo-hub-d50-5g-zh-cn
luci-i18n-exigo-hub-d50-5g-zh-tw
luci-i18n-filemanager-de
luci-i18n-filemanager-es
luci-i18n-filemanager-pl
luci-i18n-filemanager-ru
luci-i18n-filemanager-zh-cn
luci-i18n-filemanager-zh-tw
luci-i18n-firewall-de
luci-i18n-firewall-es
luci-i18n-firewall-fr
luci-i18n-firewall-it
luci-i18n-firewall-pl
luci-i18n-firewall-ru
luci-i18n-firewall-vi
luci-i18n-firewall-zh-cn
luci-i18n-firewall-zh-tw
luci-i18n-internet-detector-de
luci-i18n-internet-detector-es
luci-i18n-internet-detector-fr
luci-i18n-internet-detector-it
luci-i18n-internet-detector-pl
luci-i18n-internet-detector-ru
luci-i18n-internet-detector-vi
luci-i18n-internet-detector-zh-cn
luci-i18n-internet-detector-zh-tw
luci-i18n-ledtrig-rssi-es
luci-i18n-ledtrig-switch-es
luci-i18n-ledtrig-usbport-es
luci-i18n-lite-watchdog-de
luci-i18n-lite-watchdog-es
luci-i18n-lite-watchdog-fr
luci-i18n-lite-watchdog-it
luci-i18n-lite-watchdog-pl
luci-i18n-lite-watchdog-ru
luci-i18n-lite-watchdog-vi
luci-i18n-lite-watchdog-zh-cn
luci-i18n-lite-watchdog-zh-tw
luci-i18n-modemband-de
luci-i18n-modemband-es
luci-i18n-modemband-fr
luci-i18n-modemband-it
luci-i18n-modemband-pl
luci-i18n-modemband-ru
luci-i18n-modemband-vi
luci-i18n-modemband-zh-cn
luci-i18n-modemband-zh-tw
luci-i18n-modemdata-de
luci-i18n-modemdata-es
luci-i18n-modemdata-fr
luci-i18n-modemdata-it
luci-i18n-modemdata-pl
luci-i18n-modemdata-ru
luci-i18n-modemdata-vi
luci-i18n-modemdata-zh-cn
luci-i18n-modemdata-zh-tw
luci-i18n-package-manager-de
luci-i18n-package-manager-es
luci-i18n-package-manager-fr
luci-i18n-package-manager-it
luci-i18n-package-manager-pl
luci-i18n-package-manager-ru
luci-i18n-package-manager-vi
luci-i18n-package-manager-zh-cn
luci-i18n-package-manager-zh-tw
luci-i18n-ports-status-mod-de
luci-i18n-ports-status-mod-es
luci-i18n-ports-status-mod-fr
luci-i18n-ports-status-mod-it
luci-i18n-ports-status-mod-pl
luci-i18n-ports-status-mod-ru
luci-i18n-ports-status-mod-vi
luci-i18n-ports-status-mod-zh-cn
luci-i18n-ports-status-mod-zh-tw
luci-i18n-qfirehose-de
luci-i18n-qfirehose-es
luci-i18n-qfirehose-fr
luci-i18n-qfirehose-it
luci-i18n-qfirehose-pl
luci-i18n-qfirehose-ru
luci-i18n-qfirehose-vi
luci-i18n-qfirehose-zh-cn
luci-i18n-qfirehose-zh-tw
luci-i18n-sms-tool-js-de
luci-i18n-sms-tool-js-es
luci-i18n-sms-tool-js-fr
luci-i18n-sms-tool-js-it
luci-i18n-sms-tool-js-pl
luci-i18n-sms-tool-js-ru
luci-i18n-sms-tool-js-vi
luci-i18n-sms-tool-js-zh-cn
luci-i18n-sms-tool-js-zh-tw
luci-i18n-used-channels-de
luci-i18n-used-channels-es
luci-i18n-used-channels-fr
luci-i18n-used-channels-it
luci-i18n-used-channels-pl
luci-i18n-used-channels-ru
luci-i18n-used-channels-vi
luci-i18n-used-channels-zh-cn
luci-i18n-used-channels-zh-tw
luci-i18n-wifihistory-de
luci-i18n-wifihistory-es
luci-i18n-wifihistory-fr
luci-i18n-wifihistory-pl
luci-i18n-wifihistory-ru
luci-i18n-wifihistory-zh-cn
luci-i18n-wifihistory-zh-tw
luci-lib-base
luci-lib-ip
luci-lib-jsonc
luci-lib-nixio
luci-lib-uqr
luci-light
luci-lua-runtime
luci-mod-admin-full
luci-mod-network
luci-mod-status
luci-mod-system
luci-proto-ipv6
luci-proto-ppp
luci-proto-quectel
luci-proto-wireguard
luci-ssl
luci-theme-bootstrap
mkf2fs
modemband
modemdata
mtd
netifd
nftables-json
odhcp6c
odhcpd-ipv6only
openwrt-keyring
pciids
pciutils
ppp
ppp-mod-pppoe
procd
procd-seccomp
procd-ujail
px5g-mbedtls
qfirehose
qlog
quectel-CM-5G-M
r8169-firmware
resolveip
rpcd
rpcd-mod-file
rpcd-mod-iwinfo
rpcd-mod-luci
rpcd-mod-rrdns
rpcd-mod-ucode
rssileds
sms-tool
sysfsutils
sysinfo
terminfo
ubi-utils
uboot-envtools
ubox
ubus
ubusd
uci
uclient-fetch
ucode
ucode-mod-digest
ucode-mod-fs
ucode-mod-html
ucode-mod-log
ucode-mod-lua
ucode-mod-math
ucode-mod-nl80211
ucode-mod-rtnl
ucode-mod-ubus
ucode-mod-uci
ucode-mod-uloop
uhttpd
uhttpd-mod-ubus
unzip
urandom-seed
urngd
usb-modeswitch
usbids
usbutils
usign
webconsole
wifi-scripts
wireguard-tools
wireless-regdb
wpad-basic-mbedtls
wsdd2
wwan
zlib
```
</details>
