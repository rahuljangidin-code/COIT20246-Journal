# Week 04 – Network Technologies

## Task 5 – View ARP Table (Optional)

The ARP table was viewed using the `arp -a` command in Windows PowerShell after communicating with other devices on the local network, such as accessing websites and pinging the default gateway.

A screenshot of the ARP table has been captured and uploaded as evidence.

### Reachable Devices Identified

Two reachable devices identified from the ARP table are:

1. **Device 1**
   - IP Address: 192.168.1.1
   - MAC Address: xx-xx-xx-xx-xx-xx
   - Explanation: This device is the network router (default gateway). It is reachable because it is responsible for forwarding traffic between the local network and the internet.

2. **Device 2**
   - IP Address: 192.168.1.5
   - MAC Address: xx-xx-xx-xx-xx-xx
   - Explanation: This device is another host connected to the same local area network. It appears in the ARP table because recent communication occurred between this device and the computer.

### ARP Table Screenshot

![ARP Table Screenshot](week4-task5-arp-table.png)
