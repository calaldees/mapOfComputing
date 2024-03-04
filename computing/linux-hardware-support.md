Linux Hardware Support
======================

Linux has an uphill battle working with hardware vendors

* [The growing image-processor unpleasantness](https://lwn.net/SubscriberLink/904776/aa7224d94a7c43c0/)
    * Modern processors have hardware image processing modules `IPU6 `. Linux drivers are hard to do. Existing API's `V4L2 ` need reworking for new features `KCAM`. Intel do not release how to interface with this hardware (probably because they outsourced the module to another company and don't have the rights to it). This will take many years for Linux to support it.
    * > "CPU performance is impacted by a daemon doing buffer copying for v4l2 loopback device" (only 720p)
* [HDMI Forum to AMD: No, you can’t make an open source HDMI 2.1 driver](https://arstechnica.com/gadgets/2024/02/hdmi-forum-to-amd-no-you-cant-make-an-open-source-hdmi-2-1-driver/) - Linux users can't hit the same resolutions and speeds as Windows—or DisplayPort.
