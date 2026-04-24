# Networking Basics

### 1. Network: 
  A pathway through which different devices are connected to each other. 

### 2. Internet: 
  A huge network consisting of many small networks all connected together. The Internet is itself a public network that connects much smaller networks called private networks. 

### 3. IP address: 
  The Internet Protocol address is a way through which a host (device) can be identified on a network. 
  * It can be associated with another device without changing the IP address itself.
  * Two devices cannot have the same IP address simultaneously.
  *  A device can have both public and private addresses at the same time depending on which type of network they are on.

 **Private IP address:** It is the address assigned to your devices by your local router. It isn't visible outside the LAN.
 
<img width="644" height="372" alt="image" src="https://github.com/user-attachments/assets/3bc97dca-35fb-45d4-b3a0-36452e39c546" />  

**Public IP address:** It is the address assigned to your router by your ISP (Internet Service Provider). To the rest of the internet, it looks like every device on your router is coming from this single public IP. 

### 4. IPv4 (Internet Protocol version 4):
  This is the veteran system created in the 1980s. It uses a 32-bit address format. 
  * **Format:** Four sets of numbers separated by dots (e.g., 192.168.1.1). 
  * **Capacity:** It can only create about 4.3 billion unique addresses. 
Today, with billions of people owning multiple phones, laptops, and smart devices, we have officially run out of unique IPv4 addresses. 

### 5. IPv6 (Internet Protocol version 6) 
   This is a replacement. It uses a 128-bit address format. 

* **Format:** Eight groups of four hexadecimal characters separated by colons (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334). 

* **Capacity:** It can create 340 undecillion addresses (that’s a 340 followed by 36 zeros). 

* **The Solution:** This is so many addresses that we could assign a unique IP to every single atom on the surface of the Earth and still have addresses left over. We will never run out again. 

### 6. MAC Address: 
  The Media Access Control address is an unchangeable, permanently unique identifier assigned to a device within its LAN at the time of its manufacture. It is a burned-in address (BIA) in hardware. It is a 12-character hexadecimal number grouped in twos and separated by colons called separators. **00:1A: 2B:3C:4D:5E**   
  Once the data travels out of the LAN, the MAC addresses are replaced by the public IP addresses of devices.  
We can change the MAC address of a device temporarily within the LAN for privacy/security reasons through two ways: 

  (i) MAC Spoofing: It's like telling a network that your device has a different MAC address by masking the actual one.  
 (ii) MAC Randomization: Generating a fake MAC address through every new router the device passes, not to expose the device’s actual location within the same LAN. 

***Note:*** *The spoofed/randomized MAC address can be any address (or even a duplicate). It is in the software unlike BIA (the actual MAC address).*

### 7. LAN:
  A Local Area Network is a collection of devices connected together in one physical location, such as a home, office, or school. It can range from a small home network with two users to an enterprise network with thousands of users and devices.  

### 8. Wireless AP:
  A Wireless Access Point is a networking hardware device that allows Wi-Fi-capable devices (like your laptop or phone) to connect to a wired network. It is a bridge between the "air" (wireless signals) and the "cable" (the wired ethernet network). 

### 9. Bandwidth: 
  It is the capacity (speed) of a network connection. It tells us how many “chunks” of data can be pushed at a time through the network. It is measured in Mbps. 

### 10. Ping:
  Ping (or latency) is the time taken for the ICMP (Internet Control Message Protocol) packets to complete one round-trip. It measures the RTT (round-trip time) of the “echo request” packet to leave your device and “echo reply” packet to come back to the same device. Echo packets travel by jumping (hops) through several routers. If any router is slow or busy, the ping goes up. It is measured in ms. 

* ***Ping Vs. Bandwidth:*** *Ping is the reaction time, or how much time it takes for a data packet to travel from a device to a server and back. Whereas bandwidth is the number of lanes on a highway. More lanes mean more cars (data) can travel at the same time.*
