# shellinabox
OpenWrt packet of shellinabox

$ cd ~/reboot/lede-U35WF/package

$ git clone https://github.com/arvati/shellinabox.git

$ cd shellinabox

$ git pull

$ cd ..

$ cd ..

$ make menuconfig

Select shellinabox in Network category

$ make package/shellinabox/compile

$ make package/shellinabox/install

$ make package/index

$ ls bin/packages/mipsel_24kc/base/shellinabox*

$ ls bin/packages/mipsel_24kc/base/busybox*

$ ls bin/packages/mipsel_24kc/base/libopenssl*

$ ls bin/packages/mipsel_24kc/base/zlib*
