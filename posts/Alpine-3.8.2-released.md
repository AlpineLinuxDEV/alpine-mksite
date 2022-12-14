---
title: 'Alpine 3.8.2 released'
date: 2018-12-20
---

Alpine Linux 3.8.2 released
===========================

The Alpine Linux project is pleased to announce the immediate
availability of version 3.8.2 of its Alpine Linux operating system.

This is a bugfix release of the v3.8 stable branch, based on
linux-4.14.89 kernels and it contains bugfixes.

The full lists of changes can be found in the [git
log](http://git.alpinelinux.org/cgit/aports/log/?h=v3.8.2) and [bug
tracker](http://bugs.alpinelinux.org/versions/128).

Git Shortlog
------------

<pre>
Andy Postnikov (11):
      community/php7: security upgrade to 7.2.10
      main/apache2: security upgrade to 2.4.35 (CVE-2018-11763)
      main/icecast: security upgrade to 2.4.4 (CVE-2018-18820)
      main/nginx: security upgrade to 1.14.1
      main/ghostscript: security upgrade to 9.26 (CVE-2018-19409)
      main/lighttpd: upgrade to 1.4.52
      community/php7: security upgrade to 7.2.13
      community/php5: security upgrade to 5.6.38 (CVE-2018-17082)
      community/php5: backport dependency fixes from edge
      main/nginx: upgrade to 1.14.2
      community/php5: security upgrade to 5.6.39

Carlo Landmeter (3):
      main/dnsmasq: add BRIDGE_ADDR_EXTRA support to initd
      main/mqtt-exec: initd use supervise-daemon
      main/mqtt-exec: keep exec_user for backwards compatibility

Euan Harris (1):
      main/libjpeg-turbo: Backport fix for CVE-2018-1152

Fabian Affolter (1):
      main/py-requests: upgrade to 2.19.1

Henrik Riomar (3):
      main/nfs-utils: drop build dep on libnfsidmap-dev
      main/xen: upgrade to 4.10.2
      main/open-vm-tools: fix reboot and halt

Ian Douglas Scott (1):
      main/gcc: patch to remove call to glibc-specific function in Ada library

J0WI (4):
      community/openjdk8: security upgrade to 3.9.0 (java 8u181b13)
      main/openssl: security upgrade to 1.0.2q - CVE-2018-0734 - CVE-2018-5407
      main/clamav: security upgrade to 0.100.2
      main/ghostscript: security fixes (CVE-2018-17961, CVE-2018-18073, CVE-2018-18284)

Jake Buchholz (1):
      main/linux-vanilla: enable NFS v4.1 & v4.2

Jakub Jirutka (7):
      community/lua-http: fix wrong depend on lua5.[12]-compat5.3
      main/ruby: security upgrade to 2.5.2
      main/one-context: upgrade to 0.5.5
      main/nodejs: security upgrade to 8.14.0
      main/nginx: upgrade module http-fancyindex to v0.4.3
      main/nginx: upgrade module http-lua to 0.10.13
      main/nginx: upgrade module http-vod to 1.24

Jean-Louis Fuchs (1):
      main/duplicity: missing pkgrel bump

Kaarle Ritvanen (10):
      main/lua-ossl: support encrypted keys
      main/lua-asn1: upgrade to 2.2.0
      main/strongswan: increase guard time
      main/tunnel: backport from edge
      main/dmvpn: backport from edge
      main/dmvpn: upgrade to 1.0.0
      main/py-django-haystack: fix dependencies
      main/mariadb-c-connector: fix socket path
      main/awall: upgrade to 1.5.2
      main/busybox: do not hang on DAD failure

Leonardo Arena (20):
      main/libsndfile: security fix (CVE-2018-13139)
      main/ulogd; fix patch and checksum
      main/strongswan: security fix (CVE-2018-17540)
      main/libexif: security fix (CVE-2017-7544)
      main/hylafax: security fix (CVE-2018-17141)
      community/nextcloud: upgrade to 13.0.7
      community/ffmpeg: use built-in RTMP support
      main/dnsmasq: fix typo
      main/curl: security fixes
      main/tiff: security fixes
      main/pango: security fix (CVE-2018-15120)
      main/lcms2: security fix (CVE-2018-16435)
      main/ghostscript: security upgrade to 9.25 (CVE-2018-16802)
      main/spice: security upgrade to 0.14.1 (CVE-2018-10873)
      main/spice-protocol: upgrade to 0.12.14
      community/zabbix: upgrade to 3.4.15
      community/postgresql-bdr-extension0.9: downgrade to 0.9.0 to maintain compatibility with earlier Alpine versions
      community/nextcloud: upgrade 13.0.8
      community/nextcloud: upgrade to 14.0.4
      community/nextcloud: additional apps are required to run upon installation of main package

Markus Heimbach (1):
      main/postfix: Adding missing m4 build dependency

Marvin Steadfast (1):
      main/libssh: security upgrade 0.7.6 - CVE-2018-10933

Natanael Copa (113):
      main/libjpeg-turbo: backport security fix (CVE-2018-11813)
      main/openssl1.0: upgrade to 1.0.2p
      main/libnfsidmap: remove due to merge with nfs-utils
      community/webkit2gtk: security upgrade to 2.20.4
      community/libreoffice: fix tread stack size issue
      main/strongswan: backport security fix (CVE-2018-16151, CVE-2018-16152)
      main/strongswan: bump pkgrel
      main/nss: backport fix for CVE-2018-12384
      main/gd: backport security fix for CVE-2018-1000222
      main/libx11: security upgrade to 1.6.6
      main/hylafax: fix secfixes comment
      main/libexif: fix secfixes comment
      main/tzdata: upgrade to 2018f
      main/libxml2: backport security fixes
      main/git: security upgrade to 2.18.1 (CVE-2018-17456)
      community/wireshark: security upgrade to 2.4.10
      main/xorg-server: security fix (CVE-2018-14665)
      main/rp-pppoe: update pkgdesc
      main/db: add secfixes comment for unaffected CVEs
      community/go: upgrade to 1.10.5
      main/linux-vanilla: upgrade to 4.14.73
      main/linux-vanilla: upgrade to 4.14.78
      main/linux-vanilla: enable drivers for Huawei Taishan 2280
      main/linux-vanilla: upgrade to 4.14.81
      main/linux-vanilla: upgrade to 4.14.82
      main/linux-rpi: upgrade to 4.14.82
      community/virtualbox-guest-modules-vanilla: rebuild against kernel 4.14.82-r0
      main/dahdi-linux-vanilla: rebuild against kernel 4.14.82-r0
      main/devicemaster-linux-vanilla: rebuild against kernel 4.14.82-r0
      main/drbd9-vanilla: rebuild against kernel 4.14.82-r0
      main/spl-vanilla: rebuild against kernel 4.14.82-r0
      main/xtables-addons-vanilla: rebuild against kernel 4.14.82-r0
      main/zfs-vanilla: rebuild against kernel 4.14.82-r0
      testing/aws-ena-driver-vanilla: rebuild against kernel 4.14.82-r0
      testing/ipt-netflow-vanilla: rebuild against kernel 4.14.82-r0
      testing/wireguard-vanilla: rebuild against kernel 4.14.82-r0
      main/imagemagick: disable openmp
      main/pango: fix secfixes comment
      main/openjpeg: security fixes (CVE-2017-17480,CVE-2018-18088)
      main/libmspack: security upgrade to 0.8_alpha
      community/salt: security upgrade to 2018.3.3 (CVE-2018-15750,CVE-2018-15751)
      community/salt: add secfixes comment
      main/cabextract: security upgrade to 1.9 (CVE-2018-18584)
      main/cabextract: fix secfixes comment
      main/linux-vanilla: upgrade to 4.14.84
      community/virtualbox-guest-modules-vanilla: rebuild against kernel 4.14.84-r0
      main/dahdi-linux-vanilla: rebuild against kernel 4.14.84-r0
      main/devicemaster-linux-vanilla: rebuild against kernel 4.14.84-r0
      main/drbd9-vanilla: rebuild against kernel 4.14.84-r0
      main/spl-vanilla: rebuild against kernel 4.14.84-r0
      main/xtables-addons-vanilla: rebuild against kernel 4.14.84-r0
      main/zfs-vanilla: rebuild against kernel 4.14.84-r0
      testing/aws-ena-driver-vanilla: rebuild against kernel 4.14.84-r0
      testing/ipt-netflow-vanilla: rebuild against kernel 4.14.84-r0
      testing/wireguard-vanilla: rebuild against kernel 4.14.84-r0
      main/linux-rpi: upgrade to 4.14.84
      main/git: security fix (CVE-2018-19486)
      community/roundcubemail: security upgrade to 1.3.8 (CVE-2018-19206)
      main/bind: security upgrade to 9.12.3 (CVE-2018-5741)
      main/lua5.3: upgrade to 5.3.5
      main/lua5.3: fix linenoise patch
      main/libao: security fix for CVE-2017-11548
      main/perl: security upgrade to 5.26.3
      main/linux-vanilla: upgrade to 4.14.85
      community/virtualbox-guest-modules-vanilla: rebuild against kernel 4.14.85-r0
      main/dahdi-linux-vanilla: rebuild against kernel 4.14.85-r0
      main/devicemaster-linux-vanilla: rebuild against kernel 4.14.85-r0
      main/drbd9-vanilla: rebuild against kernel 4.14.85-r0
      main/spl-vanilla: rebuild against kernel 4.14.85-r0
      main/xtables-addons-vanilla: rebuild against kernel 4.14.85-r0
      main/zfs-vanilla: rebuild against kernel 4.14.85-r0
      testing/aws-ena-driver-vanilla: rebuild against kernel 4.14.85-r0
      testing/ipt-netflow-vanilla: rebuild against kernel 4.14.85-r0
      testing/wireguard-vanilla: rebuild against kernel 4.14.85-r0
      main/linux-rpi: upgrade to 4.14.85
      community/jenkins: upgrade to 2.121.3
      main/ghostscript: update secfixes comment
      main/tiff: security upgrade to 4.0.10
      main/openrc: fix hostname script
      commit/php7: fix merge error
      main/linux-vanilla: upgrade to 4.14.88
      community/virtualbox-guest-modules-vanilla: rebuild against kernel 4.14.88-r0
      main/dahdi-linux-vanilla: rebuild against kernel 4.14.88-r0
      main/devicemaster-linux-vanilla: rebuild against kernel 4.14.88-r0
      main/drbd9-vanilla: rebuild against kernel 4.14.88-r0
      main/spl-vanilla: rebuild against kernel 4.14.88-r0
      main/xtables-addons-vanilla: rebuild against kernel 4.14.88-r0
      main/zfs-vanilla: rebuild against kernel 4.14.88-r0
      testing/aws-ena-driver-vanilla: rebuild against kernel 4.14.88-r0
      testing/ipt-netflow-vanilla: rebuild against kernel 4.14.88-r0
      testing/wireguard-vanilla: rebuild against kernel 4.14.88-r0
      main/linux-rpi: upgrade to 4.14.88
      community/go: upgrade to 1.10.7
      main/linux-vanilla: upgrade to 4.14.89
      community/virtualbox-guest-modules-vanilla: rebuild against kernel 4.14.89-r0
      main/dahdi-linux-vanilla: rebuild against kernel 4.14.89-r0
      main/devicemaster-linux-vanilla: rebuild against kernel 4.14.89-r0
      main/drbd9-vanilla: rebuild against kernel 4.14.89-r0
      main/spl-vanilla: rebuild against kernel 4.14.89-r0
      main/xtables-addons-vanilla: rebuild against kernel 4.14.89-r0
      main/zfs-vanilla: rebuild against kernel 4.14.89-r0
      testing/aws-ena-driver-vanilla: rebuild against kernel 4.14.89-r0
      testing/ipt-netflow-vanilla: rebuild against kernel 4.14.89-r0
      testing/wireguard-vanilla: rebuild against kernel 4.14.89-r0
      main/linux-rpi: upgrade to 4.14.89
      main/varnish: upgrade to 6.0.2
      community/pdns-recursor: security upgrade to 4.1.8
      main/py-packaging: move from community due to py-sphinx
      main/samba: security upgrade to 4.8.8
      main/py-sphinx: add all runtime deps to makedepends
      community/cfengine: fix needed symlinks
      main/imagemagick: upgrade to 7.0.7.39
      ==== release 3.8.2 ====

Roberto Oliveira (2):
      community/keepalived: upgrade to 2.0.5
      main/py-typing: move from community

Thomas Liske (1):
      main/ipset: fix reloading of existing ipsets

Timo Ter??s (1):
      main/asterisk: security upgrade to 15.6.1

raschi.alex@gmail.com (1):
      community/gst-plugins-bad: enable opus support

</pre>
