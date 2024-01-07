AV1
===

* [Technical Overview of AV1 Spec](https://github.com/QuPengfei/Technical-Overview-Of-AV1-Spec)
* [The AV1 video codec gains broader hardware support](https://fullystacked.net/posts/av1/) October 2023

HOLY SHIT AV1!!!
from [av1_presentation.pdf](https://www.mlug-au.org/lib/exe/fetch.php?media=av1_presentation.pdf)
```
ffmpeg -i input.mp4 -c:v libsvtav1 -preset 4 -qp 50 -sc_detection true -pix_fmt yuv420p10le -g 240 -sn -c:a libopus -ac 2 svt-av1.webm
```
