Evolution of Computer Graphics
==============================

* [[history-of-graphics]]

Part 1 - 2D Graphics as pixel data
-------------------------------

Computer displays are all broken into describe chunks called `pixels`

[8x8 pixel graphic](https://www.google.com/search?q=8x8+smile)

* Gameboy - 160 x 144 - [Super Mario World](https://www.youtube.com/watch?v=sdSpTUHIGgw)
* NES - 256 x 240
* Playstation 1 - 256 x 224
* DVD - 720 x 480
* 1080p - 1920 x 1080


```python
    def draw_sprite(data, width=8):
        """
            --####--
            -#----#-
            #-#--#-#
            #------#
            #-####-#
            #------#
            -#----#-
            --####--

            As linear pixel data
            --####---#----#-#-#--#-##------##-####-##------#-#----#---####--
        """
        for line_number in range(len(data)//width):
            print(data[line_number * width:(line_number + 1) * width])

    sprite_data = '--####---#----#-#-#--#-##------##-####-##------#-#----#---####--'
    draw_sprite(sprite_data)
```

The process of taking chunks from data from one memory location and copying it to another is called `blit-ing` [bit block transfer](https://en.wikipedia.org/wiki/Bit_blit).

* [MicroMages NES Game - 8x8 Sprite explanation](https://youtu.be/ZWQ0591PAxM?t=162)
* [computer-vision-basics-in-microsoft-excel](https://github.com/amzn/computer-vision-basics-in-microsoft-excel)
* [Designing 2D graphics in the Japanese industry](https://vgdensetsu.tumblr.com/post/179656817318/designing-2d-graphics-in-japan-from-the-late-70s)
    * western world used core tools - japan used home grown tech
    * historical look at tools and artwork
    * [When graphic designers from Taito, SNK and other companies used a joystick to draw dot by dot.](https://videogamesdensetsu.tumblr.com/post/160230210495/when-graphic-designers-from-taito-snk-and-other)

Part 2 - 3D Graphics as pixels
------------------------------

### Wireframe 3D - Drawing of lines

* algorithms
    * [[line-drawing]] Bresenham

Examples
* [BattleZone](https://www.youtube.com/watch?v=e5_MXGkLvpI) PC
* [Red Alarm](https://www.google.com/search?q=red+alarm+virtual+boy)
    * [Red Alarm Review](http://www.nintendolife.com/reviews/2009/04/red_alarm_retro)
* [Elite](https://youtu.be/1ZT6ItqZ2xc) BBC

### Filled Polygons

[Polygon Filling Algorithm](https://www.tutorialspoint.com/computer_graphics/polygon_filling_algorithm.htm) [[polygon]]

Examples
* [Carrier Command](https://youtu.be/NvpcGs-NJPw?t=408) Amiga
* [Elite](https://youtu.be/z_ei6LSj8IM?t=33) PC

Draw triangles in the correct order

The processes of taking triangle geometry and drawing it as pixels is called `rasterisation`

### Textured Mapping

* [Software Texture Mapping](https://youtu.be/RyYEGdGwnFs)
* [Quake 1 - Different renderers](https://www.youtube.com/watch?v=6STlawZarcU)
* [What makes the graphics of the original PlayStation look so unique?](https://www.youtube.com/watch?v=DyjalwYBJNQ) YouTube 15min

Quake 1 engine was sold/licensed to game developers.


Part 3 - Modern 3D Graphics Chipsets
------------------------------------

3D Graphics Cards are a completely separate computer inside your computer that is dedicated to drawing triangles.

Modern game programmers do NOT write code to 'blit sprites' or 'rasterise triangles'. These are solved problems.
Modern game programmers use graphics library's and hardware.

Mobile chipsets - 200 Million triangles per second - source [imagination graphics benchmark guide](https://www.imgtec.com/blog/consumer-guide-to-graphics-benchmarks/)

Part 4 - The furture
--------------------

* [Enhancing Photorealism Enhancement](https://intel-isl.github.io/PhotorealismEnhancement/)
    * Use of AI to apply photo-realism to game footage (GTA5)
    * Temprolly stable
* [8k 3D Holographic display](https://lookingglassfactory.com/8k)

Further Reading
---------------

* [A Brief History of Graphics](https://www.youtube.com/watch?v=QyjyWUrHsFc) 45min documentary - Ahoy
* [fabiensanglard.neta](https://fabiensanglard.neta) - Game code teardowns
    * [Another World](http://fabiensanglard.net/another_world_polygons/index.html)
* [VoxelSpace](https://github.com/s-macke/VoxelSpace)
* [CGA 1024 Colors](https://int10h.org/blog/2015/04/cga-in-1024-colors-new-mode-illustrated/)
    * [[cga]]
* [haiku_icons](http://blog.leahhanson.us/post/recursecenter2016/haiku_icons.html)
* [History of Computer graphics](https://www.youtube.com/watch?v=QyjyWUrHsFc)
* [How Prince of Persia Defeated Apple II's Memory Limitations | War Stories | Ars Technica](https://www.youtube.com/watch?v=sw0VfmXKq54)
* [Freescape 3D engine for 8bit computers](https://paleotronic.com/2019/04/26/3d-adventures-with-freescape/)
* [Ray Tracing In Notepad.exe At 30 FPS](http://kylehalladay.com/blog/2020/05/20/Rendering-With-Notepad.html)
* [Grafica Obscura](http://graficaobscura.com/) - a collection of computer graphics hacks 70's to 90's #papercraft [[maths]]
Link to algorithms.md for pixelart resizing

[//begin]: # "Autogenerated link references for markdown compatibility"
[history-of-graphics]: history-of-graphics.md "History of Graphics"
[line-drawing]: line-drawing.md "line-drawing"
[polygon]: polygon.md "Polygon"
[cga]: cga.md "cga"
[maths]: maths.md "Maths"
[//end]: # "Autogenerated link references"