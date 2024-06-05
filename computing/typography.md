Typography
==========

* [User Interface Typography](https://imperavi.com/books/ui-typography/)
    * > This book is about how to do good user interface typography, from basic things and principles to building layout and various design elements. The book has hundreds of illustrations that explain every nuance and principle. 
* [The Elements of Typographic Style Applied to the Web](http://webtypography.net/)
    * > For too long typographic style and its accompanying attention to detail have been overlooked by website designers, particularly in body copy. In years gone by this could have been put down to the technology, but now the web has caught up. The advent of much improved browsers, text rendering and high resolution screens, combine to negate technology as an excuse.
* [Font size is useless; let’s fix it](https://tonsky.me/blog/font-size/)
* [Please Stop Using Grey Text](https://tangledweb.xyz/please-stop-using-grey-text-3d3e71acfca8)
* [Time to upgrade your monitor](https://tonsky.me/blog/monitors/) - Font Rasterisation on modern OS's
* Concept
    * [Continuous Typography](https://maxkoehler.com/posts/continuous-typography/) - Notes toward a continuous framework for screen typography
        * Typography on the web is differnt to paper. We make lots of decisions about fonts. We could have functions to select these
* [Please Stop “Fixing” Font Smoothing](https://usabilitypost.com/2012/11/05/stop-fixing-font-smoothing/)
    * Critique on `-webkit-font-smoothing` CSS
    * > for main portions of text where readability is paramount please leave the default setting alone and let the operating system handle the smoothing.
* [Bunny Fonts](https://fonts.bunny.net/about)
    * GDPR open drop in replacement for google fonts

### Fonts for coding

* [Input - Fonts for code](https://input.djr.com/preview/)
    * Live preview of coding font - LOADS of cool options - great for exploring typography
* [CodingFont](https://www.codingfont.com/)
    * Asks you to compare two fonts and helps you find your _perfect_ coding font
    * Mine was `Inconsolata`
* [programmingfonts.org](https://www.programmingfonts.org/)
    * fonts for coding with previews


Fonts
-----

* Raster Fonts
    * Mario's Lab [Rendering like it's 1996 - Bitmap fonts and DOS](https://marioslab.io/posts/rendering-like-its-1996/dos-nostalgia/)
        * Testing graphics throughput on a 486 (touch video memory ONCE as you have limited bandwidth)
    * [Arcade Game Typography](https://readonlymemory.vg/shop/book/arcade-game-typography/)
    * [ZX Origins](https://damieng.com/typography/zx-origins) - 8x8 mono bitmap fonts
    * [Tiny bitfield based text renderer](https://www.onirom.fr/wiki/blog/25-09-2022_tiny_bitfield_based_text_renderer/)
        * Tiny nanofont3x4 - the samllest typeface with upper and lowercase latters
        * Anders de Flon created a 3x3 font but it is upper case only.
        * [dotsies](https://dotsies.org/) a 1x5 font to replace glyphs!
    * [NFG's Arcade Font Engine](https://nfggames.com/games/fontmaker/lister.php)
        * https://github.com/calaldees/TeachProgramming/blob/12614dd3905ea15d45d1ce9d7cf58f5423a29b2d/teachprogramming/static/projects/game/pygame_zoomer.py#L100
        * ```python
            def font_loader(filename, sequence='ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789', size=8, font_name='aof2'):
                """
                Load fonts for use with PyGame
                https://nfggames.com/games/fontmaker/index.php
                https://nfggames.com/system/arcade/arcade.php/y-pabom/z-0/x-ABCDEFGHIJKLMNOPQRSTUVWXYZ01234567890
                """
                filename = Path(filename)
                # Download font if it does not exist
                if not filename.exists():
                    filename.parent.mkdir(parents=True, exist_ok=True)
                    url = f'https://nfggames.com/system/arcade/arcade.php/y-{font_name}/z-{(size/8)-1}/x-{sequence}'
                    with urllib.request.urlopen(url) as url_request, filename.open(mode='wb') as filehandle:
                        filehandle.write(url_request.read())
                # Load font to dict
                image = pygame.image.load(str(filename))
                return MappingProxyType({
                    character: image.subsurface((i*size, 0, size, size))
                    for i, character in enumerate(sequence)
                })
          ```
        * TODO: Add support for wraparound black and white fonts. See TeachProgramming enhancement
    * [BitmapFonts](https://github.com/ianhan/BitmapFonts/blob/main/README.md)
        * My collection of bitmap fonts pulled from various demoscene archives over the years
    * [hoard-of-bitfonts](https://github.com/robhagemans/hoard-of-bitfonts/)
        * Black and white fonts in text files for retro computers
    * [Raster CRT Typography (According to DEC)](https://www.masswerk.at/nowgobang/2019/dec-crt-typography)
        * html5 canvas simulator for raster fonts on CRT
    * [opengameart.org pixel font pack](https://opengameart.org/content/bitmap-font-pack)
    * [Game Font Forensics](https://int10h.org/blog/2024/02/game-font-forensics/)
        * Comparing fonts on the Apple2 and IBM-PC
* TrueType (only black and white flat)
    * Rendering
        * [Writing a TrueType font renderer](https://axleos.com/writing-a-truetype-font-renderer/)
            * Amazing breakdown of the process and querks
    * Fonts
        * [Lexend](https://www.lexend.com/)
            * [github](https://github.com/ThomasJockin/lexend)
            * See [[Accessibility]]
        * [evangelion](https://fontsinuse.com/uses/28760/neon-genesis-evangelion)
        * [Helvetica: feature-length documentary](https://www.hustwit.com/helvetica)
        * [Inter](https://rsms.me/inter/) - Inter is a typeface carefully crafted & designed for computer screens
* Uniwidth/Multiplex/Duplexed/Equal-width
    * [Uniwidth typefaces for interface design](https://uxdesign.cc/uniwidth-typefaces-for-interface-design-b6e8078dc0f7)
* Monospace
    * [Coding with Character](https://realdougwilson.com/writing/coding-with-character)
        * Monospace fonts for coding with personality
        * If you spend all day looking at code, letters, and characters—why not make it fun?
    * [Dev Fonts](https://devfonts.gafi.dev/) - free monospace font comparison
    * [comic-mono](https://dtinth.github.io/comic-mono-font/)
    * [Typography in 8 bits: System fonts](https://damieng.com/blog/2011/02/20/typography-in-8-bits-system-fonts/)
        * Spectrum, c64, amstrad, apple2, atari 400/800, bbc, msx
    * [oldschool-pc-fonts](https://int10h.org/oldschool-pc-fonts/readme/)
        * [fontlist](https://int10h.org/oldschool-pc-fonts/fontlist/)
        * [romfont](https://github.com/spacerace/romfont)
        * [ibm-prototype](https://int10h.org/blog/2016/03/olympiad-ibm-prototype-fonts-unearthed/)
    * [rewtnull/amigafonts](https://github.com/rewtnull/amigafonts) - Faithfully remade multi platform Amiga fonts in Amiga aspect 
* Custom
    * [Making a font](https://kokorobot.ca/site/making_a_font.html)
        * for comicbooks
    * Handwriting
        * [font based on my handwriting](https://sachachua.com/blog/2020/06/pythonfontforgeorg-i-made-a-font-based-on-my-handwriting/)
        * [Coding my Handwriting](https://www.amygoodchild.com/blog/cursive-handwriting-in-javascript)
    * [Creating a handwritten TrueType font in Linux](https://gordonlesti.com/creating-a-handwritten-truetype-font-in-linux/)
        * example and instructions
        * > I always wanted to create a font out of my handwritten letters and in this small tutorial I will show you the way I have done it with the help of FontForge, Inkscape and GIMP.
    * [calligrapher.ai](https://www.calligrapher.ai/)
        * AI generated handwriting
* Exotic
    * [Nabla: Isometric font](https://nabla.typearture.com/)
    * [Teranoptia](https://www.tunera.xyz/fonts/teranoptia/)
        * build monsters with fonts (no letters, just using font as a glyph)
* Color fonts
    * [Google Color Fonts](https://fonts.google.com/knowledge/introducing_type/introducing_color_fonts)
* [Variable Fonts](https://v-fonts.com/)
    * Fonts with variables!
    *  v0.2 A simple resource for finding and trying variable fonts 

Text is Hard
------------
* [The strangely difficult problem of drawing a box around text](https://blog.battlefy.com/the-strangely-difficult-problem-of-drawing-a-box-around-text-e6a70bdf6bb9)
* [Simple software things that are actually very complicated](https://www.construct.net/en/blogs/ashleys-blog-2/simple-software-things-1587)

Security with fonts
-------------------

* [Fonts are still a Helvetica of a Problem](https://www.canva.dev/blog/engineering/fonts-are-still-a-helvetica-of-a-problem/) - CVEs in three strange places and the unique problem of safely processing and handling fonts.
    * Lots of formats - lots of attack area - examples of POC of [[security]] vulnerabilities
    * Postscript, OpenType, TrueType, SVG. So many formats

Physical Typography
===================

* [Remnants of a Legendary Typeface Have Been Rescued From the River Thames](https://news.artnet.com/art-world/doves-typeface-2454807)
    * Doves Type was thrown into the water a century ago, following a dispute between its creators.
    * (amazing story of recovering lead type from the Thames. Mudlarks are professionals who recover historical items from rivers. got port of london authority)

[//begin]: # "Autogenerated link references for markdown compatibility"
[Accessibility]: accessibility.md "Accessibility"
[security]: security.md "Hacking and Security"
[//end]: # "Autogenerated link references"