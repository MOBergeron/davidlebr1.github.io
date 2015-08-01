---
layout: post
title:  "PoliCTF - John In The Middle"
date:   2015-07-13 22:30
categories: polictf2015
summary : This is a forensic challenge for 100 points.
tags: security ctf polictf2015 forensic
---

First, we had to download the [pcap file]({{ site.url }}/files/PoliCTF2015/John-In-The-Middle/john-in-the-middle.pcap) with the following message *Can John hijack your surfin'? :)*
We know that a pcap file is a extracted file from Wireshark. So, we need to analyze the network packets. 

My first reflex with Wireshark is to verify if I can extract file that are transfered between the client and the server in the pcap file.

The file that were extract was the website file of [polictf.it](http://polictf.it)

After, I found that the logo.png on the website was different with the one in the extract file. 

So, I use Stegsolve to analyze the image. 

Finally, the flag was in the image. 

The image logo.png with the flag hidden :

![Logo without flag]({{ site.url }}/files/PoliCTF2015/John-In-The-Middle/logo.png)

The image with the flag:

![Logo with flag]({{ site.url }}/files/PoliCTF2015/John-In-The-Middle/flag.png)


flag{J0hn_th3_Sn1ff3r}


