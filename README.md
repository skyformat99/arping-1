# arping

Variant of arping tool which is a part of iputils(Based on version
iputils-s20121221), customized IP/MAC address of source/destination is allow to
be used.

Usage: arping [-fqbuDUAV] [-c count] [-w timeout] [-I device] [-s source-ip] [-S source-mac] [-d desc-mac] destination
  -f : quit on first reply
  -q : be quiet
  -b : keep broadcasting, don't go unicast
  -u : always unicast
  -D : duplicate address detection mode
  -U : Unsolicited ARP mode, update your neighbours
  -A : ARP answer mode, update your neighbours
  -V : print version and exit
  -c count : how many packets to send
  -w timeout : how long to wait for a reply
  -i interval : interval in seconds between sending packets
  -I device : which ethernet device to use
  -s source-ip : source ip address
  -S source-mac : source MAC address
  -d dest-mac : MAC address of destination
  destination : ask for what ip address


Example:
  arping -I eth0 -c 2 -i 1 -s 1.1.1.1 -S 44:44:44:44:44:44 -d 88:88:88:88:88:88 2.2.2.2

