# Activity Overview

As a security analyst, you must capture and filter network traffic in a Linux environment. You also need to understand basic network interface concepts. In this lab, you’ll use tcpdump to capture network traffic, save it to a packet capture (p-cap) file, and examine the captured data to focus on specific traffic types.

## Scenario

You are a network analyst using tcpdump to capture and analyze live network traffic from a Linux virtual machine. Your Linux user account, `analyst`, is already logged into a terminal. A sample packet capture file exists in your home directory to answer questions at the end of the lab.

Steps in the lab:

1. Identify network interfaces to capture packet data.  
2. Use tcpdump to filter live network traffic.  
3. Capture network traffic with tcpdump.  
4. Filter captured packet data for analysis.  

**Note:** Use Google Chrome or Mozilla Firefox for optimal lab performance.

## Start the Lab

1. Click the green **Start Lab** button.  
2. A Linux shell will appear for performing lab steps.  
3. Follow the **End your Lab** instructions when finished.

## Task 1 – Identify Network Interfaces

1. List available interfaces using ifconfig:
sudo ifconfig

csharp
Copy code
2. Example output shows `eth0` as the Ethernet interface. This will be used for packet capture.  
3. Identify interfaces using tcpdump:
sudo tcpdump -D

markdown
Copy code

## Task 2 – Inspect Network Traffic on an Interface

1. Capture live traffic from `eth0`:
sudo tcpdump -i eth0 -v -c5

markdown
Copy code
Options:  
- `-i eth0`: capture on interface eth0  
- `-v`: verbose output  
- `-c5`: capture 5 packets  

2. Example tcpdump output shows timestamp, protocol, source and destination, TCP flags, checksum, sequence and acknowledgment numbers, window size, and packet length.  

## Task 3 – Capture Network Traffic to a File

1. Capture only web traffic (TCP port 80) into a file:
sudo tcpdump -i eth0 -nn -c9 port 80 -w capture.pcap &

markdown
Copy code
Options:  
- `-nn`: disable name resolution  
- `-c9`: capture 9 packets  
- `port 80`: filter HTTP traffic  
- `-w capture.pcap`: save to file  
- `&`: run in background  

2. Generate HTTP traffic with curl:
curl opensource.google.com

markdown
Copy code
3. Verify capture:
ls -l capture.pcap

shell
Copy code

## Task 4 – Filter Captured Packet Data

1. View packet header data:
sudo tcpdump -nn -r capture.pcap -v

markdown
Copy code
Options:  
- `-nn`: disable name resolution  
- `-r capture.pcap`: read file  
- `-v`: verbose output  

2. View hexadecimal and ASCII packet data:
sudo tcpdump -nn -r capture.pcap -X

markdown
Copy code
Option `-X` displays packet data in hex and ASCII for pattern analysis or forensic inspection.

## Test Your Understanding

1. Capture 3 packets on any interface with verbose:
- `sudo tcpdump -c3 -i any -v`  
2. The `-i` option indicates: network interface to monitor  
3. The `-v` option includes: verbose information  
4. Identify available interfaces for capture: `sudo tcpdump -D`  

## Conclusion

You practiced:

- Identifying network interfaces  
- Capturing network data with tcpdump  
- Interpreting tcpdump output  
- Saving and reading packet capture files  

You are ready to capture and analyze network traffic effectively.
