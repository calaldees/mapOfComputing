Font Rendering
====

* alphapixeldev: [SDF vs MSDF vs Slug vs Rive vs Texture Atlas: GPU Text Rendering Explained](https://alphapixeldev.com/sdf-vs-msdf-vs-slug-vs-rive-gpu-text-rendering/) 2026
    * Patent for _Slug_ GPU font rendering was made to public in 2026 and implemented by Slughorn [[c++]]
    * Rather than rending the whole font to 64x64 textures and interpolating
    * Per horizontal scan line - take only the curves that cross that scanline - count the intersections line-crossing algorithm.
    * Great for hardware motion graphics

* [Font Rendering from First Principles](https://mccloskeybr.com/articles/font_rendering.html) 2026
* [The strangely difficult problem of drawing a box around text](https://blog.battlefy.com/the-strangely-difficult-problem-of-drawing-a-box-around-text-e6a70bdf6bb9)
* [Simple software things that are actually very complicated](https://www.construct.net/en/blogs/ashleys-blog-2/simple-software-things-1587)
* [Text Rendering Hates You](https://faultlore.com/blah/text-hates-you/) 2019
    * Rasterising text is HARD
    * Tech characters overlap
    * Aliasing is hell - subpixel rendering?
* [Please Stop “Fixing” Font Smoothing](https://usabilitypost.com/2012/11/05/stop-fixing-font-smoothing/)
    * Critique on `-webkit-font-smoothing` CSS
    * > for main portions of text where readability is paramount please leave the default setting alone and let the operating system handle the smoothing.
* Font rendering used to be in kernel space in windows WTF!
* [Time to upgrade your monitor](https://tonsky.me/blog/monitors/) - Font Rasterisation on modern OS's
* [Rendering Crispy Text On The GPU](https://osor.io/text) Rasterisation
    * The mother document! This breakdown is AMAZING!
    * [HN Comments](https://news.ycombinator.com/item?id=44265233)

[c++]: c%2B%2B.md "c++"
