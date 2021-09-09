# openwrt-reinstall
Script to automatically reinstall your openwrt when you sysupgrade

This is something to achieve what we have in Debian when we apt dist-upgrade
but on openwrt.

When we sysupgrade an openwrt machine we typically loose all installed extra
packages and end up with a basic install again. This script takes care of
reinstallation of the extra packages you want by specifying them on a config
file and enabling the reinstall service before doing the sysupgrade.

More info on my initial post on reinstall on my blog at:
http://blog.manty.net/2021/08/openwrt-dist-upgrade-or-how-to-update.html

