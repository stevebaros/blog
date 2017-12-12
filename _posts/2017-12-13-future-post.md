---
layout: post
title: Future Post
description: Google VR view allows developer to host VR content very easily with various platforms, including Android, iOS and Web. In this post, I embedded some sample VR view widgets on my Jekyll page hosted on Github. All you need is a Google Cardboard to experience the 3D immersive world.
tags: event-hub
---

<style>
.highlight-left {margin-left: 0}
</style>

[Google VR view](https://developers.google.com/vr/concepts/vrview) allows developer to host VR content very easily with various platforms, including Android, iOS and Web. The content being hosted can be image or video, mono or stereo. Developer is also able to embed hotspot to allow user interaction with the VR content. More importantly, the [VR view repository](https://github.com/googlevr/vrview) is open-source on Github.

In this post, I embedded some sample VR view widgets on my Jekyll page hosted on Github. All you need is a [Google Cardboard](https://vr.google.com/cardboard/) to experience the 3D immersive world!

## Showcase

### Mono 360 Image

<div id="vrview-image-mono"></div>

Image courtesy: [Google VRView example](http://googlevr.github.io/vrview/examples/gallery/index.html)

### Stereo 360 Image

<div id="vrview-image-stereo"></div>

Image courtesy: [Google VRView webpage](https://developers.google.com/vr/concepts/vrview)

If you are using a browser on **PC**, the mono and stereo 360 images are rendered in the same way. Differences come when you are using a browser on a **phone**, and by clicking the Cardboard button on the widget. The script will redirect you to the Cardboard viewing mode.

Mono 360 image is rendered on a sphere, and pixel will be placed at the same focal distance. With stereo 3D image, the [vergence](https://en.wikipedia.org/wiki/Vergence) of your eye will give you binocular vision.

## VRView on Jekyll Blog

Enabling VRView content on your Jekyll blog is very straight-forward.

**1. Build a local version of VRView**

Clone the repository of [Google VRView](https://github.com/googlevr/vrview), and compile as instructed.

**2. Copy the vrview folder into your jekyll folder**

**3. Declare the place holder for vrview content in your blog file**

{% highlight html %}
<div id="vrview-image-mono"></div>
{% endhighlight %}{: .highlight-left }

**4. Add scripts to load desired content into the vrview widget**

{% highlight javascript %}
<script>
window.addEventListener('load', onVrViewLoad);
function onVrViewLoad() {
  var vrView1 = new VRView.Player('#vrview-image-mono', {
    image: '/public/image/vrview-taj-mahal.jpg',
    is_stereo: false,
    width: '100%',
    height: 360
  });
}
</script>
{% endhighlight %}{: .highlight-left }

The VRView Player class has some parameters that you can play with, for example, video looping, stereo mode control. The detailed list can be found on [Google VR view website](https://developers.google.com/vr/concepts/vrview-web).

**5. Build and experience!**

Because Github page allows [CORS (Cross-Origin Resource Sharing)](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing), the content you upload to your Github repo can be accessed, for example, the video in vrview.

## How about Video?

A little bit tricky! **Sometimes it does not play.**

<div id="vrview-video-stereo"></div>

Video courtesy: [Google VRView example](http://googlevr.github.io/vrview/examples/video/index.html)

## Another Trick

VRView is able to handle requests as well.

### Image Request

This is another mono 360 image, available with vrview examples:

[http://longqian.me/vrview?image=../public/image/vrview-chichen-itza.jpg](http://longqian.me/vrview?image=../public/image/vrview-chichen-itza.jpg)

### Video Request

The following link will play the same video as in the previous section.

[http://longqian.me/vrview?video=../public/video/congo_2048.mp4&is_stereo=true](http://longqian.me/vrview?video=../public/video/congo_2048.mp4&is_stereo=true)

Player parameter can be appended to the URI with **&** symbol, and multiple parameters can be concatenated.

Bloging should be **COOL** in the VR era. 

Thanks for reading! <img class="inline" src="/public/LQ144x144.png" alt="LQ" style="width:1.5rem;height:1.5rem;" />



<script src="/vrview/build/three.min.js"></script>
<script src="/vrview/build/vrview.min.js"></script>
<script>
window.addEventListener('load', onVrViewLoad1)
window.addEventListener('load', onVrViewLoad2)
window.addEventListener('load', onVrViewLoad3)
function onVrViewLoad1() {
  var vrView1 = new VRView.Player('#vrview-image-mono', {
    image: '/public/image/vrview-taj-mahal.jpg',
    is_stereo: false,
    width: '100%',
    height: 360
  });
}

function onVrViewLoad2() {
  var vrView2 = new VRView.Player('#vrview-image-stereo', {
    image: '/public/image/vrview-coral.jpg',
    is_stereo: true,
    width: '100%',
    height: 360
  });
}

function onVrViewLoad3() {
  var vrView3 = new VRView.Player('#vrview-video-stereo', {
    video: '/public/video/congo_2048.mp4',
    is_stereo: true,
    width: '100%',
    height: 360,
    default_yaw: 180,
    loop: true
  });
}

</script>

