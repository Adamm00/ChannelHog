# ChannelHog

## About

Monitor and force maximum 5GHz bandwidth for Asus RT-AX88U as seen on [SmallNetBuilder](url)

Tired of badly configured neighbours and DFS cutting your wireless bandwidth in half? Then this is the script for you!

ChannelHog will monitor your current 5GHz channel bandwidth on a daily basis and if it detects anything lower then 160MHz it will restart the 5Ghz radio. This script also includes optional Discord notification support.

**Note:** *Your clients will temporarily be disconnected from the 5GHz band in the event of a restart, this usally takes 1-2 minutes and occurs at 4.45am.*

## Donate

This script will always be open source and free to use, but if you want to support future development you can do so by [Donating With PayPal.](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=BPN4LTRZKDTML)

## Usage

To open the menu its as simple as;

```Shell
sh /jffs/addons/channelhog/channelhog.sh
```

[![ChannelHog GUI](https://i.imgur.com/YfYthFy.png "ChannelHog GUI")](https://i.imgur.com/YfYthFy.png  "ChannelHog GUI")

[![ChannelHog Notifications](https://i.imgur.com/jG5tY40.png "ChannelHog Notifications")](https://i.imgur.com/jG5tY40.png  "ChannelHog Notifications")

## Installation

In your favorite SSH Client;

```Shell
mkdir -p /jffs/addons/channelhog && /usr/sbin/curl -s "https://raw.githubusercontent.com/Adamm00/ChannelHog/master/channelhog.sh" -o "/jffs/addons/channelhog/channelhog.sh" && chmod 755 /jffs/addons/channelhog/channelhog.sh && sh /jffs/addons/channelhog/channelhog.sh install
```