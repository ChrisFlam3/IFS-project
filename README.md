# IFS-project
IFS fractal explorer

Compressed IFS fractal explorer which uses multithreading or GPU CUDA for calculations. 
Rendering pipeline implemented via SFML lib with few OpenGL tweaks, 
UI implemented using nuklear lib with SFML as rendering and baking engine.

Keep in mind that GPU rendering is only avalible for NVIDIA GTX series and won't work with any AMD GPU.
High quality render is avalible only in 2k resolution, it is advised to use resonable samples amount, in most cases 10 billions should be more than enough.

Expected render times for HQ:
GPU-under 5 min
Multithreading (depends on physical core number and speed), for 4 cores around 20-30 min
Single core (depends), for 3.2 GHz around 1.5h

REMEMBER:Multithreading and GPU rendering affect only HQ, preview mode will bypass any multithreading.

For now explorer supports only 8 bit grayscale but renders could be easily colored using postprocess softs.

![ScreenShot](https://raw.github.com/ChrisFlam3/IFS-project/IFS-project/render_examples/juliaedited.png)
