Volumetric Display
==================

* https://github.com/AncientJames/multivox?tab=readme-ov-file
    * https://youtu.be/pcAEqbYwixU?si=coC53nkR2O6v1QwN&t=987
    These are the two most frequent comments on this video.

The low resolution is linked to the need for extremely high refresh rates. The panels need to sweep around fast enough that persistence of vision turns them into a single image, and as they sweep around they need to light up a different pattern of light at every position in the volume. The panels have a resolution of 128x64, so to get an even density in 3D they need to be able to generate 2πr = 400 dots around the circumference - they need to update 400 times per revolution. At 25 fps for the volume, shared between two sceens, that's 400 x 25 / 2 =  5000 fps. These panels can handle this, in part because they allow very low level control and you can trade colour depth for refresh rate.
If you increase it to a 1920x1080 OLED, it now needs 3000 slices - 37500 fps. The fastest gaming monitor is 500 fps. This is no longer the realm of a cheap hobby project.

As for a vacuum - it's a very appealing idea. The shiny dome is reminiscent of a piece of CRT era technology, and the thin wide screens rotating at high speed look very unaerodynamic. But inside the dome the air quickly ends up rotating at the same rate as the rest of the mechanism. It's reaching its design speed with the motor at less than half duty cycle. Even if it were practical to make the whole thing airtight, it doesn't solve a problem that I currently have.
The sound it makes doesn't come from inside the dome but from the motor in the base, and soundproofing that has a lot in common with soundproofing a PC. Isolate moving parts from the case, apply sound deadening materials, use a lower rpm motor. Don't block up the vents and prevent any airflow inside it.