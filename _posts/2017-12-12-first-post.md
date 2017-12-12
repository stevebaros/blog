---
layout: post
title: First Post
description: Augmented World EXPO 2017 was held in Santa Clara, with 4700 attendee, 351 speakers, 212 exhibitors. AWE is the largest industrial exhibition in the field of Augmented Reality. Some Virtual Reality players attend the conference too. As the concept of AR getting more and more popular, it is time to check out how these concepts come to life. In this post, I will share some of the highlights that I saw during the EXPO.   
tags: event-hub
---

<p class="full-width">
<img src="/public/image/awe-2017.jpg" width="100%" align="right"/>
</p>

This year, the annual [Augmented World EXPO](http://www.augmentedworldexpo.com/) was hosted in Santa Clara, California, and attracted 4700 attendee, 351 speakers, 212 exhibitors. Everyone witnessed the momentum of AR technology with these numbers keep growing year to year. However, many of us is aware of the fact that it still takes time for all the fantasy to be realized, which is dependent on the hardware, software tools, and content. This post highlights some of the exciting or cool stuff I saw during AWE 2017.

## Hardware

Frankly, there are not a lot of serious players in this section. Let's see what they have brought us in AWE 2017.

### Microsoft HoloLens

In AWE, Microsoft has a large booth, demonstrating a medical application using [HoloLens](https://www.microsoft.com/en-us/hololens). It is not something new in terms of hardware. However, when you walk around the exhibition, you probably noticed how many of the demos are built on top of HoloLens. It is still the best Mixed Reality headset in the market.

Just a few days ago, Microsoft released several other affordable [Mixed Reality headsets](https://developer.microsoft.com/en-us/windows/mixed-reality). All of them powered by Microsoft mixed reality software architecture. **The giant is building its mixed reality ecosystem, from hardware, to software, to app store.**

### Meta 2

[Meta](https://www.metavision.com/) is another serious player in building head-mounted displays. At Day 2 of AWE, the CEO of Meta, Meron Gribetz, shared with us about the history of Meta, and some exciting applications on Meta 2. [AR Workspace](https://www.vrfocus.com/2017/06/ar-workspace-for-meta-introduced-at-awe-2017/) is trying to bring HMD to everyone everyday use, where you can **WORK**, efficiently, wearing Meta 2. Meta shipped its SDK with the device, to perform inside-out tracking, communication with mobile phone, etc. The most exciting part of Meta 2 is its 90 degree diagonal field-of-view, which makes Augmented Reality more immersive.

Hope Meta could ship our order soon!

### ODG

<p class="full-width">
<img src="/public/image/odg.jpg" width="100%" align="right"/>
</p>

[ODG](https://shop.osterhoutgroup.com/) is a very experienced smartglass designer and manufacturer. In AWE, they demonstrated its new products: R-8 and R-9. Some insights are built into the new devices: larger FOV, more powerful, cheaper. They also started to create its software architecture for inside-out tracking. But the performance is not yet as good as HoloLens. In addition, [R-7HL](https://www.cnet.com/news/smart-glasses-ar-odg-r7-hl-torture-test/) is introduced for harzardous manufacturing environment. 

### Daqri

<p class="full-width">
<img src="/public/image/daqri-helmet.jpg" width="60%" align="right"/>
</p>

[Daqri](https://daqri.com/) is planning big for AR headset, including smart helmet, smart glass, and a head-up display for car. The inside-out tracking is also built with its device, but not as good as HoloLens yet. I tried out the smart helmet and the head-up display.

### Epson Moverio

[Epson Moverio](https://epson.com/moverio-augmented-reality) brought two new devices: BT-350 and BT-2200. As a user of BT-200 and BT-300, I instantly found out that the optics system of all Moverio BT serires are the same, except for the slight difference in resolution. The display is very sharp, but lack field-of-view. From my opinion, Epson's product are very well focused in terms of potential customer groups. BT-2000 and BT-2200 are for manufacturers, like Daqri smart helmet. BT-300 and BT-350 are for individual use as a head-up display. It is not intended for the usecase of AR Workspace, on the contrary to Meta 2.

### Intel Alloy

<p class="full-width">
<img src="/public/image/intel-alloy.jpg" width="100%" align="right"/>
</p>

[Intel](https://www.intel.com/content/www/us/en/homepage.html) has been in this field for years, featuring its sensing technology, [RealSense](https://www.intel.com/content/www/us/en/architecture-and-technology/realsense-overview.html). Based on its inside-out tracking technology, Intel at AWE demonstrated its [Project Alloy](https://newsroom.intel.com/chip-shots/intel-unveils-project-alloy/). In the video, the indoor environment is mapped to a virtual gaming environment, and two players are playing VR games in the room. The tracking performance is quite well from the video.

In my opinion, Project Alloy is the closeset VR headset to ideal. It is untethered, and does not require external tracking systems. With such platform, VR content providers should be confident that their product can be delivered well to customers.

### Others

- [DeepOptics](http://www.deepoptics.com/do_site/) brought an interesting hardware to the market: an additional lens that can be put on top of traditional stereoscopic lenses, to dynamically adjust the focal plane. It is very useful to mitigate [vergence-accommodation conflict](http://longqian.me/2016/10/05/vergence-accommodation-conflict-vac/).
- [Massless](http://www.massless.io/) creates a pen as controller of AR and VR content. Check out the [video](https://venturebeat.com/2017/06/04/massless-lets-you-write-with-a-pen-in-virtual-reality/).
- [Kopin](http://www.kopin.com) offers a very thin [VR headset](http://lightspeedpr.com/vr-headsets-shrinking-in-size/), compared to the bulky Oculus and HTC Vive.




## Software Tools

### Vuforia

[Vuforia](https://vuforia.com/) has been supporting the majority of AR applications on the market. Vuforia provides the tracking library that is compatible with almost all platforms. They started from image tracking that relies on features and patterns in the image. On the stage of AWE, Vuforia demonstrated its [Project Chalk](https://developer.vuforia.com/projectchalk).

Project Chalk is built on inside-out featureless tracking, and can be built into daily-use application to enable remote communication. I think cross-platform is the strongest point of Vuforia. A few days ago, Apple released its inside-out tracking SDK, [ARKit](https://developer.apple.com/arkit/). Appearently, Apple does a huge amount of work after its acquisition of [metaio](http://www.metaio.eu/) two years ago. It will be exciting to see what will happen in the SDK market.

### Wikitude

[Wikitude](http://www.wikitude.com) eyes at the same market as Vuforia. Their team won the **Best Developer Tool** of AWE this year. I haven't used their product, so I cannot comment on its tracking performance.

### Manomotion

[Manomotion](http://manomotion.com/) provides hand tracking SDK, based on mono-camera. Their demo works very well in general, except for some error in the depth. This is very hard to conquer without additional help from other sensors. Leap Motion is more well-known for the same purpose of hand tracking. They do have additional sensors. Manomotion can be integrated with mobile AR applications, which is a under-addressed market.


## Content Providers

### Sandbox

<p class="full-width">
<img src="/public/image/sandbox.jpg" width="60%" align="right"/>
</p>

The [Sandbox](https://arsandbox.ucdavis.edu/) from UC Davis is very fun to play with. It is projector-based augmented reality application. I was amazed at how well the system is engineered and tuned to be both accurate and stable.


However, I didn't see many content providers in AWE, which on the other hand, demonstrated the fact that hardware and software for AR is still not ready yet. In my opinion, content providers are the key to the life or death of a certain technology. Even if the hardware is cool to use, it needs to be useful for the public, and content providers create useful things.

I hope augmented reality content providers will be gathered at AWE soon, and that's the real era of Augmented Reality.


<p class="full-width">
<img src="/public/image/awe-2017-pano.jpg" width="100%" align="right"/>
</p>



Thanks for reading! <img class="inline" src="/public/LQ144x144.png" alt="LQ" style="width:1.5rem;height:1.5rem;" />

