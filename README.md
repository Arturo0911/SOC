# Network Traffic Analysis


## Tcpdump Fundamentals


Tcpdump is a command-line packet sniffer that can directly capture and interpret data
frames from a file or network interface. It was build for user on any Unix-like operating system
and had a Windows twin called Windump. It is a potent and straighforward tool used on most Unix-based systems. 
It does not require a GUI and cna be used through any terminal or remote connection, such as SSH. Nevertheless,
this tool can seem overwhelming at first


### Basic capture options

Below is a table of basic Tcpdump switches we can use to modify how or captures run. These switches can be chained
together to craft how the tool outpu is shown to use in STDOUT an dwhat is saved to the capture file. This is not an exhaustive
list, and there are many more we can use, but these are the most common and valuable


| Switch Command | Result                                      |
| -------------- | -------------------------------------------- |
| D              | Will display any interfaces available to capture from. |
| i              | Selects an interface to capture from. (e.g., -i eth0) |
| n              | Do not resolve hostnames. |
| nn             | Do not resolve hostnames or well-known ports. |
| e              | Will grab the ethernet header along with upper-layer data. |
| X              | Show contents of packets in hex and ASCII. |
| XX             | Same as X but will also specify ethernet headers. (like using Xe) |
| v, vv, vvv     | Increase the verbosity of output shown and saved. |
| c              | Grab a specific number of packets, then quit the program. |
| s              | Defines how much of a packet to grab. |
| S              | Change relative sequence numbers in the capture display to absolute sequence numbers. (e.g., 13248765839 instead of 101) |
| q              | Print less protocol information. |
| r file.pcap    | Read from a file. |
| w file.pcap    | Write into a file. |





