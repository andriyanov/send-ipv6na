send-ipv6na
===========

Sends ICMPv6 NA message(s) to given destination

Tested on FreeBSD only. Written in Perl, using RAW sockets and Socket/Socket6 modules.

===========

usage: $0 [ OPTIONS ] ip6addr
Sends ICMPv6 NA message(s) to given destination.

valid options are:
 -d --to      destination IPv6 address (default: $opt_dest)
 -m --mac     send given MAC in target link-layer address option
 -c --count   number of retransmissions (infinite: 0; default: $opt_count)
 -d --delay   sleep N seconds between retransmissions
 -v --verbose
 -h --help
