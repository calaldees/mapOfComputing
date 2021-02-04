Shaders
=======

* [The Book of Shaders](https://thebookofshaders.com/) - a gentle step-by-step guide through the abstract and complex universe of Fragment Shaders
* [shadertoy.com](https://www.shadertoy.com/) - Build and Share your best shaders with the world and get Inspired
    * [Winding Menger Tunnel](https://www.shadertoy.com/view/4scXzn)
* [Pixel Shaders in Windows Terminal](https://github.com/microsoft/terminal/tree/main/samples/PixelShaders)

HLSL

The language we use to write pixel shaders is called HLSL. It's a C-like language, with some restrictions. You can't allocate memory, use pointers or recursion. What you get access to is computing power in the teraflop range on decently recent GPUs. This means writing real-time raytracers or other cool effects are in the realm of possibility.