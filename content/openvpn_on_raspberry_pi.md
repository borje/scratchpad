+++
author = "Börje Granberg"
date = "2016-01-01T12:30:22+01:00"
description = "OpenVPN on Raspberry Pi"
#draft = true
keywords = ["raspberry pi"]
tags = ["raspberry pi", "openvpn"]
title = "OpenVPN on Raspberry Pi"
topics = ["raspberry pi"]
type = "post"
slug = "openvpn-on-raspberry-pi"

+++

For server configuration I followed the tutorial on <http://readwrite.com/2014/04/10/raspberry-pi-vpn-tutorial-server-secure-web-browsing>.

For client configuration I followed <http://readwrite.com/2014/04/11/building-a-raspberry-pi-vpn-part-two-creating-an-encrypted-client-side>.

The big problem was that I was not at home when I started this work, so to be able to open the openvpn port in the firewall I had to tunnel the VPN traffic over SSH. For this I followed this tutorial <https://redfern.me/tunneling-openvpn-through-ssh/>.
