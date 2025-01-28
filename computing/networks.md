Networks
========

* [[IPv6]]

* ["just disconnect the internet" argument](https://computer.rip/2024-07-31-just-disconnect-the-internet.html) 2024
    * It cant be done - we are connected. Threat vectors still exists in air gaps. 
    

* [[internet]]
* [[slow-network]]
* [High Performance Browser Networking](https://hpbn.co/) - eBook
    * Brilliant all-round protocols and network hardware

* Explained from first principles - [Internet](https://explained-from-first-principles.com/internet/)

Great table from link above

|Name |Purpose |Endpoints |Identifier |Example|
|-|-|-|-|-|
|Application layer |Application logic |Application-specific resource |Application-specific |HTTP|
|Security layer |Encryption and authentication |One or both of the parties |X.509 subject name |TLS|
|Transport layer |Typically reliable data transfer |Operating system processes |Port number |TCP|
|Network layer |Packet routing across the Internet |Internet-connected machines |IP address |IP|
|Link layer |Handling of the physical medium |Network interface controllers |MAC address |Wi-Fi|


* [[networking_physical_layer]]

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

* [[nagles]] algorithm

* [TCP/IP illustrated](https://www.amazon.co.uk/TCP-Illustrated-Protocols-Addison-Wesley-Professional-ebook/dp/B00666M52S) Fall, Kevin R. 2011
    * Volume 1: The protocols
    * Volume 2: The implementation
    * [vlebooks](https://www.vlebooks.com/Vleweb/Product/Index/194281)
* [[udp]]
* [[tcp]]
* [[websockets]]
* [[http]]
* [[wake-on-LAN]]

https://thesquareplanet.com/blog/how-the-internet-works/


* My Analogy:
    * A (home) router is a suite of network services.
        * Routers often contain: Network gateway, DHCP, Ethernet switch, ADSL modem and a Wireless Access Point (which also manages it's own keys).
    * In short.
        * WAP == Professional component to bridge wireless and Ethernet.
        * Router (in the context of the home) == a range of components combined for home use. a WAP is part of it's suite
    * a (home) router has a WAP as part of it. This is not helped by the fact that a (commercial) router is very different and is the logic to direct traffic to multiple nodes (using RIP for routing tables and creating self healing network). This is not what (home) routers do. So already the terminology is confusing.
    * Any simplification will create misconceptions.
    * I think the best way I can convey this to young people is (very carefully) using the analogy of 'transport infrastructure'. "How would you get to Disneyland Florida?" ... you would not just walk in the right direction ... it would take you days and days of walking and eventually you would reach the UK coast. You would use a car to go to a train station and then the airport to another airport and then a bus at the other end. Some of your family could take a later train and a different plane that takes another route, but your family would all end up together in Disnyland at some point.
    * Networks are lots of different technologies: (wifi, ADSL (copper), ehternet, transatlatic fiberoptic). Together they all form a network that can transport data.
    * Like transport infrastructure: Walking, cycling, bus, trains, airplanes, boats; are all ways of transporting a person. ...
* More of my notes
    * A home router is an amalgamation of a range of network services/devices in a single box
        - An Ethernet Switch
        - A Wireless access point (to run a wireless network and (separately) bridge this network to the Ethernet switch. The wireless network and the Ethernet switch are actually two separate networks)
        - A DHCP server (for assigning ip address's to new devices)
        - a DNS pass-through (for domain name lookup)
        - Firewall (rules for incoming and outgoing traffic)
        - ADSL modem (analogue to digital conversion)
        - Internet Gateway (bridges your local network to a wider network - the outside world)
        - Web server (Linux operating system)
            * web based admin panel
    * It is not technically a "Router" as it does not have a routing table or perform route negotiation.
    * But people call it a router as it fits the concept of "passing something on to something else".




* [Beej's Guide to Network Programming - Using Internet Sockets](https://beej.us/guide/bgnet/html/)
* [Computer Networks: A Systems Approach](https://book.systemsapproach.org/) - Larry Peterson and Bruce Davie

* [Visual sound analysis of a modem connecting](https://twitter.com/BrianRoemmele/status/1330376384871501824)
    * > Consider the sound and analysis of a 33.6kbit/s dial-up modem over traditional telephone lines.


* MAC address
    * [Change your MAC address with a shell script](https://josh.works/shell-script-basics-change-mac-address)


CSMACD

Internet categorys

Low Power
---------

* [Thread - the tech we can't use or teach](https://overengineer.dev/blog/2024/05/10/thread/)
    * Thread is an IPv6 compatable low power protocol. It's built into AppleHomeHub but the licencing prohibits any hobby/education use

WiFi
----

Wifi 6


https://blog.benjojo.co.uk/post/why-is-ethernet-mtu-1500


Tools
-----

nmap
dig
[[traceroute]]
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

Learning Resources and Simulators
---------------------------------

* [Functional and Performance Analysis of Discrete Event Network Simulation Tools](https://doi.org/10.1016/j.simpat.2021.102470)
    * 23 Network Simulators for Education with summary table

* [filius-de](https://www-lernsoftware--filius-de.translate.goog/?_x_tr_sl=de&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=sc)
    * [Introduction to the world of FILIUS](https://www.lernsoftware-filius.de/downloads/Introduction_Filius.pdf) 2015 english translation

* [Open-Source Routing and Network Simulation](https://www.brianlinkletter.com/open-source-network-simulators/)
    * A guy that updates and reviews a lits of network simulators used for education
    * https://www.brianlinkletter.com/2023/02/network-emulators-and-network-simulators-2023/
    * https://www.brianlinkletter.com/2023/03/network-simulators-for-high-school-teachers/

* [pt-anywhere](https://pt-anywhere.kmi.open.ac.uk/)
    * dont host anymore - must self host
    * Cisco packet trace on web - need to host yourself (pretty narly install)

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

Virtual Networks
----------------

* [Introduction to Linux interfaces for virtual networking](https://developers.redhat.com/blog/2018/10/22/introduction-to-linux-interfaces-for-virtual-networking)


Infrastructure
--------------

* [DHCP Games with Smart Router Devices](https://www.anvilsecure.com/blog/dhcp-games-with-smart-router-devices.html)


Routing Protocols
-----------------

* YouTube [What is a ROUTER? // FREE CCNA // EP 2](https://www.youtube.com/watch?v=p9ScLm9S3B4) NetworkChuck 2020 22min YouTube
    * Layer 2 and Layer 3 ARP example with gateway and DNS
* YouTube [How RIP Works | Network Fundamentals Part 20](https://www.youtube.com/watch?v=aNV4rVLa_sc)
* [Does the Internet Route Around Damage? - Baltic Sea Cable Cuts](https://labs.ripe.net/author/emileaben/does-the-internet-route-around-damage-baltic-sea-cable-cuts/)

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
* [The James Webb Telescope’s Profound Data Challenges](https://spectrum.ieee.org/james-webb-telescope-communications) 3000x farther from Earth than Hubble—with a 25x greater download deluge - Michael Koziol - 08 Jul 2022
* [Pico-10BASE-T](https://github.com/kingyoPiyo/Pico-10BASE-T)
    * Using gpio pins to create an ethernet interface in software!

* Ripe Labs 2023 [IP: Pollution in 1/8](https://labs.ripe.net/author/franz/pollution-in-18/)
    * > The recent allocation of the 1.0.0.0/8 and 27.0.0.0/8 not only triggered a lot of media attention due to IPv4 exhaustion exceeding the 90% mark, it also sparked the curiosity of many technical folks.

[//begin]: # "Autogenerated link references for markdown compatibility"
[IPv6]: IPv6.md "IPv6"
[internet]: internet.md "Internet"
[slow-network]: slow-network.md "Slow Network"
[networking_physical_layer]: networking_physical_layer.md "Networking- Physical Layer"
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
[nagles]: nagles.md "Nagles"
[udp]: udp.md "UDP"
[tcp]: tcp.md "TCP"
[websockets]: websockets.md "WebSockets"
[http]: http.md "HTTP"
[wake-on-LAN]: wake-on-LAN.md "Wake on LAN"
[traceroute]: traceroute.md "traceroute"
[daw]: daw.md "daw"
[distributed-filesystems]: distributed-filesystems.md "distributed-filesystems"
[maps]: maps.md "Maps"
[datasets]: datasets.md "Unsorted"
[history-of-operating-systems]: history-of-operating-systems.md "History of Operating Systems"
[//end]: # "Autogenerated link references"
