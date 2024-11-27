# tcpdump4_network_traffic
Capturing and analysing packets by tcpdump

Analysising of ip address 192.168.1.165

This captured packets provide network-related details specific to the IP address 192.168.1.165. Here's what information can be obtained based on the output of the capture:
1. Type of Traffic

    Most packets in the output are ARP (Address Resolution Protocol) requests. ARP is used to map IP addresses to MAC addresses in a local network.
    There is also a UDP NetBIOS Datagram (netbios-dgm) message from LATIN-PC to the network's broadcast address (192.168.1.255), likely related to Windows network services.

2. Devices and Relationships

    The device LATIN-PC is actively communicating with other devices in the network. It is resolving the MAC addresses of:
        G3100.mynetworksettings.com (likely your router or gateway)
        Other devices on the network (192.168.1.151, 192.168.1.156, etc.).
    The 192.168.1.165 device is not generating ARP requests, suggesting it might be a passive device or less active during this capture.

3. Network Characteristics

    Broadcast Activity: Many packets involve ARP requests sent to the broadcast address, indicating a normal network discovery process where devices announce or query network neighbors.
    Traffic Type: UDP traffic over netbios-dgm suggests that the device or network has Windows file sharing or related services enabled.

4. Host Discovery

    This captured ARP requests reveal active devices in the same subnet, their possible hostnames, and their IP addresses (e.g., Joey_MoCA, Hopper3-br).
    This allow to identify and map devices on the local network.


