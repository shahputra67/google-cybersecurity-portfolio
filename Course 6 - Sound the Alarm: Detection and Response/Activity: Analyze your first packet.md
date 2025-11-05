# Activity Overview

As a security analyst, you’ll analyze network traffic to learn what type of traffic is sent to and from systems on the networks you manage.

Packet capture and analysis help security teams interpret and understand network communications. Tools like Wireshark, which has a graphical user interface (GUI), allow you to examine packet data efficiently. Wireshark helps identify patterns and apply filters to focus on relevant traffic during investigations.

In this lab, you’ll use Wireshark to inspect a sample packet capture file and filter network traffic data.

## Scenario

You are investigating traffic to a website. You will analyze a packet capture file containing traffic data from a user connecting to an internet site. You will filter the data to:

- Identify the source and destination IP addresses involved in the session.
- Examine the protocols used during the connection.
- Analyze packets to determine the type of information sent and received.

## Lab Steps Overview

1. Open the packet capture file and explore the Wireshark GUI.
2. Inspect a single packet in detail, examining protocol and data layers.
3. Apply filters to inspect packets based on criteria.
4. Filter and inspect UDP DNS traffic.
5. Apply filters to TCP packets to search for specific payload text.

**Note:** Use Google Chrome or Mozilla Firefox for optimal lab performance.

## Start the Lab

1. Click the green **Start Lab** button.
2. Click **Open Windows VM** to launch the Windows interface for the lab.
3. Login if necessary:
   - Server: localhost  
   - Username: qwiklabs  
   - Password: Password  

## Task 1 – Explore Data with Wireshark

1. Double-click the sample `.pcap` file on the Windows desktop to open it in Wireshark.
2. Maximize the Wireshark window.
3. Overview of key columns:
   - **No.**: Packet index number
   - **Time**: Timestamp
   - **Source**: Source IP address
   - **Destination**: Destination IP address
   - **Protocol**: Protocol in the packet
   - **Length**: Packet length
   - **Info**: Packet payload details

**Question:** What is the protocol of the first packet where Info starts with "Echo (ping) request"?  
- ICMP  
- TCP  
- SSH  
- HTTP  

## Task 2 – Apply a Basic Filter and Inspect a Packet

1. Enter filter: `ip.addr == 142.250.1.139` and press Enter.
2. Double-click the first TCP packet to open the details pane.
3. Explore the subtrees:
   - **Frame**: Overall packet details
   - **Ethernet II**: Source/destination MAC addresses, internal protocol
   - **Internet Protocol Version 4 (IPv4)**: Source/destination IP, internal protocol
   - **Transmission Control Protocol (TCP)**: Ports, sequence numbers, flags

**Question:** What is the TCP destination port?  
- 80  
- 53  
- 200  
- 66  

4. Inspect TCP Flags, then close the packet detail window.
5. Clear the filter using the **Clear display filter** icon.

## Task 3 – Use Filters to Select Packets

1. Filter by source IP: `ip.src == 142.250.1.139`
2. Filter by destination IP: `ip.dst == 142.250.1.139`
3. Filter by MAC address: `eth.addr == 42:01:ac:15:e0:02`
4. Inspect the first packet and examine Ethernet II and IPv4 subtrees.

**Question:** What is the protocol in the IPv4 subtree for this MAC address?  
- UDP  
- ESP  
- ICMP  
- TCP  

## Task 4 – Use Filters to Explore DNS Packets

1. Filter DNS traffic: `udp.port == 53`
2. Open the first packet, expand **Domain Name System (query)**, and review **Queries**.
3. Open the fourth packet, expand **Answers**.

**Question:** Which IP address is in the DNS query Answers for `opensource.google.com`?  
- 139.1.250.142  
- 169.254.169.254  
- 142.250.1.139  
- 172.21.224.1  

## Task 5 – Use Filters to Explore TCP Packets

1. Filter TCP port 80 traffic: `tcp.port == 80`
2. Inspect the first packet:
   - Destination IP: 169.254.169.254

**Questions:**  
- Time to Live (IPv4 subtree): 32 / 128 / 16 / 64  
- Frame Length (Frame subtree): 40 / 54 / 74 / 60 bytes  
- Header Length (IPv4 subtree): 74 / 60 / 54 / 20 bytes  
- Destination Address (IPv4 subtree): 169.254.169.254 / 239.1.250.142 / 172.21.224.2 / 142.250.1.139  

3. Filter TCP packets containing text: `tcp contains "curl"` to inspect web requests using curl.

## Conclusion

You have practiced using Wireshark to:

- Open saved packet capture files  
- View high-level packet data  
- Use filters to inspect detailed packet information  

This skill is essential for analyzing network traffic and identifying patterns relevant to security investigations.
