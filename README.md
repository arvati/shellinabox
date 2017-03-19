# shellinabox
OpenWrt packet of shellinabox

```bash
cd ~/reboot/lede-U35WF/package
git clone https://github.com/arvati/shellinabox.git
cd shellinabox
git pull
cd ..
cd ..
make menuconfig #Select shellinabox in Network category
make package/shellinabox/compile
make package/shellinabox/install
make package/index
ls bin/packages/mipsel_24kc/base/shellinabox*
ls bin/packages/mipsel_24kc/base/busybox*
ls bin/packages/mipsel_24kc/base/libopenssl*
ls bin/packages/mipsel_24kc/base/zlib*
```

At device:
```bash
opkg update
opkg install --force-checksum busybox_1.25.1-2_mipsel_24kc.ipk
opkg install --force-checksum libopenssl_1.0.2k-1_mipsel_24kc.ipk
opkg install --force-checksum zlib_1.2.11-1_mipsel_24kc.ipk
opkg install shellinabox_2.20_mipsel_24kc.ipk
```
