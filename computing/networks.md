Networks
========

* [[certificates]]
* [[dns]]
* [[error-correction]]
* [[latency]]
* [[nat]]
* [[ports]]
* [[port-scan]]
* [[protocols]]
* [[url]]

* [[information-theory]]

* [[tor]]
* [[web]]


* [TCP/IP illustrated](https://www.amazon.co.uk/TCP-Illustrated-Protocols-Addison-Wesley-Professional-ebook/dp/B00666M52S) Fall, Kevin R. 2011
    * Volume 1: The protocols
    * Volume 2: The implementation
    * [vlebooks](https://www.vlebooks.com/Vleweb/Product/Index/194281)
* [[udp]]
* [[tcp]]
* [[websockets]]
* [[http]]

https://thesquareplanet.com/blog/how-the-internet-works/

* [Beej's Guide to Network Programming - Using Internet Sockets](https://beej.us/guide/bgnet/html/)
* [Computer Networks: A Systems Approach](https://book.systemsapproach.org/) - Larry Peterson and Bruce Davie

* [Visual sound analysis of a modem connecting](https://twitter.com/BrianRoemmele/status/1330376384871501824)
    * > Consider the sound and analysis of a 33.6kbit/s dial-up modem over traditional telephone lines.


* MAC address
    * [Change your MAC address with a shell script](https://josh.works/shell-script-basics-change-mac-address)


CSMACD

Internet categorys


WiFi
----

Wifi 6


https://blog.benjojo.co.uk/post/why-is-ethernet-mtu-1500


Tools
-----

nmap
dig
traceroute
[bandwhich - Terminal bandwidth utilization tool](https://github.com/imsnif/bandwhich)

* [SonoBus](https://sonobus.net/)
    * Low latency audio streaming with VST interface
    * [[daw]]

[Human speech may have a universal transmission rate: 39 bits per second](https://www.sciencemag.org/news/2019/09/human-speech-may-have-universal-transmission-rate-39-bits-second)

[peeringdb.com](https://www.peeringdb.com/) The Interconnection Database

* [Loon](https://blog.x.company/loons-final-flight-e9d699123a96)
    * Failed project 2021 (part fo Alphabet)
    * Network infrastructure with balloons connected by optical links
    * Other project include WingX for floating wifi

* [Submarine Cable Map](https://www.submarinecablemap.com/) - The Submarine Cable Map is a free and regularly updated resource from TeleGeography.
* [opencellid.org](https://www.opencellid.org/) - The world's largest Open Database of Cell Towers


---

Cultural social
---------------

What would not exit?

* Write a letter
* Remote Learning 
  * lectures live
  * get slides later
* Video calls (work/personal)
* How without Websites?
  * Advertising
  * Buying? Call centers?
* Self checkouts
    * Prices lables on items
* Banks
    * All closing
* Lots of jobs in call centers
* Put data on disk/tape and transport by car (fasters)
    * Floppy Disk
    * Truck? faster than network


* The bad
    * Hack?
        * Lots of personal data out their
    * Information Overload?
        * expected time to reply to most messages now minuets rather than weeks



devices in home - 
end devices
intermediate devices
services

Network media
wireless
lan media
wan media
    the beem
ethernet - wifi - bluetooth - adsl - eithernet over power? - fiber?


steam streaming box
mobile phone
bluray player
desktop computer
laptop
moisture sensor under washing machine
lights?

* [NetworkDirection.net](https://networkdirection.net/) Resources to expand your networking horizons
    * Here you will find IT educational resources, specifically for networking. Whether you are a beginner or you have been in the industry for years, you will find easy to understand videos on a range of topics to suit your skill set. 
    * [Youtube: Network Fundamentals](https://www.youtube.com/watch?v=cNwEVYkx2Kk&list=PLDQaRcbiSnqF5U8ffMgZzS7fq1rHUI3Q8)
        * 26 part series
        * TCP three way handshake

* [Cisco: Courses / Packet Tracer Courses / Intro to Packet Tracer](https://www.netacad.com/courses/packet-tracer/introduction-packet-tracer)
* [Open-Source Network Simulators](https://www.brianlinkletter.com/open-source-network-simulators/)
    * [Shadow](https://shadow.github.io/)
        * an open-source network simulator/emulator hybrid
        * runs real applications like Tor and Bitcoin over a simulated Internet topology
        * light-weight, efficient, scalable, parallelized, controllable, deterministic, accurate, modular, and more!
    * [Graphical Network Simulator3](https://www.gns3.com/)
        * Graphical Network Simulator3 is open-source software and a network emulator that allows the combination of virtual and real machine devices of almost any description used to simulate composite networks.
    * [Educational Network Simulator](http://malkiah.github.io/NetworkSimulator/)
        * [github.com/malkiah/NetworkSimulator](https://github.com/malkiah/NetworkSimulator)
* [Open Network Lab](https://onl.kmi.open.ac.uk/)
    * [pt-anywhere](http://pt-anywhere.kmi.open.ac.uk/) - free online course and simulator
* [CS4G Netsim](https://netsim.erinn.io/) - simulator game
    * Netsim is a simulator game intended to teach you the basics of how computer networks function, with an emphasis on security. You will learn how to perform attacks that real hackers use, and see how they work in our simulator!

Infrastructure
--------------

* [DHCP Games with Smart Router Devices](https://www.anvilsecure.com/blog/dhcp-games-with-smart-router-devices.html)


Routing Protocols
-----------------

* [How RIP Works | Network Fundamentals Part 20](https://www.youtube.com/watch?v=aNV4rVLa_sc)

HELLO protocol?

### Distance Vector
signposts (not whole map)
BGP (Border gateway protocol - big internet stuff) runs over TCP
RIP (runs over [[udp]])
GIGRP

Distance (number of hops) - use one it thinks is better
RIP v1 should not be used - uses boardcast
RIP v2 sends to multicast 224.0.0.9 (only RIPv2 routers listening will get them) - only single hop - very efficient (immediate neighbours)
Advertise to any connected network within a range (10.0.0.0)

on routers we can see _sources_. These are other routers that have sent updates to us

Networks are not duplex all the time. Differnt adaptors for 
egress
ingress

RIP database
| network | next hop |
|-|-|
| slash address | ip of router |

`show ip route rip`

Admisistrative distance (hops the router is away)

Recommend always disable auto-summarisation (grouping) of address (this avoids conflict)

Setup a passive interface (not advertise external ??)
Set all interfaces as passive by default

Authentication of routers - imagine someone adds a new rougue router to your network and it starts advertising evil routes to syphon traffic
Keychain - cycle keys periodicolloy


### Link State
Each router has a whole map of the network
OSPF


Distributed
-----------

* [[distributed-filesystems]]


Location Services
-----------------

* [Observing my cellphone switch towers](https://fabiensanglard.net/lte/index.html)
    * See [[maps]] and [[datasets]] (opencllid)


* [DOS SMB Client Performance](http://www.os2museum.com/wp/dos-smb-client-performance/)
    * DOS TCP/IP Network stack
    * [[history-of-operating-systems]]

Unsorted
========

* [telnet BBS guide](https://www.telnetbbsguide.com)
    * List of servers you can remote into

[//begin]: # "Autogenerated link references for markdown compatibility"
[certificates]: certificates.md "Certificates"
[dns]: dns.md "DNS"
[error-correction]: error-correction.md "Error"
[latency]: latency.md "Latency"
[nat]: nat.md "NAT Network Address Translation"
[ports]: ports.md "ports"
[port-scan]: port-scan.md "port-scan"
[protocols]: protocols.md "Protocols"
[url]: url.md "URL"
[information-theory]: information-theory.md "Information Theory"
[tor]: tor.md "Tor"
[web]: web.md "Web"
[udp]: udp.md "UDP"
[tcp]: tcp.md "TCP"
[websockets]: websockets.md "WebSockets"
[http]: http.md "HTTP"
[distributed-filesystems]: distributed-filesystems.md "distributed-filesystems"
[maps]: maps.md "Maps"
[datasets]: datasets.md "datasets"
[history-of-operating-systems]: history-of-operating-systems.md "History of Operating Systems"
[//end]: # "Autogenerated link references"
