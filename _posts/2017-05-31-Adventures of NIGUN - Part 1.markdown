---
layout: post 
title: "Adventures of NIGUN. Gate 1"
date:   2017-05-31 01:08:03 +0200
categories: jekyll update
---

I got familiar with RTL-SDR for the first time around 2013. Even though there are plenty of better options, I believe that RTL-SDR has a major donation to the education of anyone who is interested in electrical engineering, communication and computer science. A $25 USB dongle and a computer combine into a very powerful tool that allows gaining hands-on experience with complex concepts of communication and DSP which used to be explained only in theory. No surprise that [some universities][ee course link] already use RTL-SDR as a major part of their DSP courses.

However...there is a major disadvantage: the RTL-SDR only supports the frequency band of 24-1700[MHz]. In fact, you can already see a performance degradation around 1500[MHz]. This means you can play nicely with commercial FM, the ISM bands below 1[GHz], lower GSM bands and even GPS at 1.575[GHz] (with some help from a LNA).   
But what about high UMTS or LTE bands? or ISM2.4? there are quite a few interesting bands and technologies which RTL-SDR is not enough for them. Yes, there are some very nice projects that [leverage some commercial down-converters][cyberexplorer link] in order to achieve those bands, but those are usually designed for one specific bands and don't support multiple bands or any dynamic change unless they are [tampered with][SUP link].

This was the point when I started thinking about a generic, dynamic down-converter for RTL-SDR. I called it NIGUN - Melody in Hebrew.  
Without any previous experience in PCB design, I started a year's journey that led me to the point of having a prototype-ready design. 
In the following posts I'm going to share my experience in designing NIGUN. As I'm going forward to prototype production, I will hopefully share the results.             

[ee course link]:https://inst.eecs.berkeley.edu/~ee123/sp16/
[SUP link]:http://www.rtl-sdr.com/a-demonstration-of-the-rtl-sdr-receiving-wifi-and-2-4-ghz-ism-with-a-modded-sup-2400-downconverter/
[cyberexplorer link]:http://blog.cyberexplorer.me/2014/01/sniffing-and-decoding-nrf24l01-and.html
