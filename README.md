# READMEL: perl-dshield-ulogd1

## Description

This Perl app is a DShield.org client. Designed to be run out of cron, this script scrapes the mysql database used by iptables/ulogd to store the firewall entries, formats the entries, then submits them to dshield.org.

The [ulogd-1.x](http://www.netfilter.org/projects/ulogd/index.html) series has entered end-of-life, so this client is probably not relevant anymore. I haven't used it in quite a while. Please pass along any issues you find.

One kind user sent in a patch a 1000 years ago, which I subsequently lost. My apologies.

## Configuration

The configurable items for this script are stored in `/etc/dshield-ulog.conf` and in `~/.dshieldrc`. It first reads the file in `/etc` then the one in your home directory.

Running `dshield-ulog -h` will give a list of options.

## Effluvia

License: GPLv2. Please see the file LICENSE.

Copyright (C) 2003-2015 John W. Palmieri.
