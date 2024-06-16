---
title: network-fundamentals
date: 2024-6-15
media_subpath: 
categories: [networking,THM,study notes]
tags: [pre-security]

---


# what is networking ??

![](https://i.pinimg.com/564x/14/73/a1/1473a15f7e5087c26dd293bc28235e6f.jpg)

> Networks are simply things connected together 

> in computing network can be formed by anywhere from 2 devices to billions connected together 

---
# what is the internet ?

> simply a giant network that consist of many small networks 



![](https://assets.tryhackme.com/additional/networking-fundamentals/intro-to-networking/what-is-the-internet/internet2.png)
_internet consist of many small netwoks_

those small networks called **private networks** where networks connecting them called **public networks "internet"** 

so , networks can be classified into :
- private network 
- public network

# identifying devices on a network

devices like humans have two things to being identified :
 - name --> IP
 - fingerprint --> MAC 

## IP address 

IP address (or **I**nternet **P**rotocol) address can be used as a way of identifying a host on a network for a period of time


![](https://tryhackme-images.s3.amazonaws.com/user-uploads/5de96d9ca744773ea7ef8c00/room-content/a0de0d68641982ddf1a8c5a9f1984c4c.png)
_**IP** is a set of numbers divided into 4 pieces we call them 4 octets, IP change from device to another in the same network , it's illegal to having same IP for two different devices in the same network_



to make a communicate understandable and more convenience **IP** Addresses follow a set of standards known as **protocols**. These protocols are the **backbone** of networking and force many devices to communicate in the same **language**,

A **public** address is used to identify the device on the Internet(**public** **network**), whereas a **private** address is used to identify a device among other devices in the **private** **network**


> if two devices in the same **private** network they will having a **different** IP address in the **private** network , but when go online to the internet they will communicate to the outside world with one **same** **public** **IP** address 

that public IP address given by ISP (internet server provide) e.g. WE egypt (LOL)

there's two types of IP versions : IPv4, IPv6 
4 -> old one e.g. 86.157.52.21

6 -> new one because many devices go online these days and there's no capacity in IPv4 for that e.g. 2a00:22c4:a531:c500:425f:cce6:c36b:f64d

version 6 have more IPs capacity 

## MAC address


![](https://tryhackme-images.s3.amazonaws.com/user-uploads/5de96d9ca744773ea7ef8c00/room-content/394caee97fb1b9f7b5a5f7a7ea0a9f71.png)
_devices have another address a physical one fixed address burned on NIC in the motherboard and it's **uniqe** wrote in hexadecimal_ 

OH nooooo it's can be **spoofed** too !! "using that in hacking stuff" to make a 
firewall passing that MAC address 

## ping (ICMP)

it's a protocol send packets to check the performance of connection between two devices in the same network 
the mechanism is simply the sender send a **ICMP echo packet** and waiting for **ICMP echo reply** from the target device 

```bash
ping 192.168.1.254
```


the respond be like :

![](https://www.firewall.cx/images/stories/icmp-echo-example.gif)
 

---
next --> intro to LAN 