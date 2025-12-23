Shaders
=======

* [An introduction to Shader Art Coding](https://www.youtube.com/watch?v=f4s1h2YETNY) YouTube 22min kishimisu
    * vectors, swizzling, global constants - this video has it all
* [shader-school](https://github.com/stackgl/shader-school) GitHub
    * A workshopper for GLSL shaders and graphics programming 
* [The Book of Shaders](https://thebookofshaders.com/) - a gentle step-by-step guide through the abstract and complex universe of Fragment Shaders
* [shadertoy.com](https://www.shadertoy.com/) - Build and Share your best shaders with the world and get Inspired
    * [Winding Menger Tunnel](https://www.shadertoy.com/view/4scXzn)
* [3D Game Shaders For Beginners](https://github.com/lettier/3d-game-shaders-for-beginners)
* [godotshaders.com](https://godotshaders.com/) - Godot Shaders is a community-driven shader library for the Godot game engine
* [Pixel Shaders in Windows Terminal](https://github.com/microsoft/terminal/tree/main/samples/PixelShaders)
* [Simulating worlds on the GPU - Four billion years in four minutes](https://davidar.io/post/sim-glsl) [[simulation]]
    * Simulating a planets development in shaders. Plate techtonics, errosion, humanity, climate change
* [Conway's Game of Life in Shader](https://js1024.fun/demos/2020#8) JS1024 2020 competition entry
    * [[cellular-automata]]
    * [[conway]]

* [Periodic Spaces](https://ianthehenry.com/posts/periodic-spaces/) One of my favorite SDF techniques is domain repetition

HLSL

The language we use to write pixel shaders is called HLSL. It's a C-like language, with some restrictions. You can't allocate memory, use pointers or recursion. What you get access to is computing power in the teraflop range on decently recent GPUs. This means writing real-time raytracers or other cool effects are in the realm of possibility.

* [NTSC-CRT](https://github.com/LMP88959/NTSC-CRT)
    * not really a shader - pure C image filter to make things look like NTSC VHS

* [🖍️ 5 ways to draw an outline: Different techniques for rendering outlines in Unity](https://ameye.dev/notes/rendering-outlines/)

* YouTube [Compute Shaders: Optimize your engine using compute / Lou Kramer, AMD](https://www.youtube.com/watch?v=0DLOJPSxJEg) 2017

[simulation]: simulation.md "Simulation"
[cellular-automata]: cellular-automata.md "Cellular Automata"
[conway]: conway.md "Conways Game of Life"

