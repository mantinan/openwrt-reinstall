# openwrt-reinstall
Script to automatically reinstall your OpenWrt when you sysupgrade

This is something to achieve what we have in Debian when we apt dist-upgrade
but on OpenWrt.

When we sysupgrade an OpenWrt machine we typically loose all installed extra
packages and end up with a basic install again. This script takes care of
reinstallation of the extra packages you want by specifying them on a config
file and enabling the reinstall service before doing the sysupgrade.

More info on my initial post on reinstall on my blog at:
http://blog.manty.net/2021/08/openwrt-dist-upgrade-or-how-to-update.html

Current version stores package status and implements a "check" parameter to
output those packages that were not installed last time reinstall was run,
so that you may add them to the config file before upgrading, and a "chen"
parameter to check and enable the service.

Last tested on OpenWrt 24.10.2
