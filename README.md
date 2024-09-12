# CUDA-RT-one-weekend-const-parameter
Modify Ray Tracing in One Weekend by Peter Shirley http://in1weekend.blogspot.com/2016/01/ray-tracing-in-one-weekend.html 
and CUDA code by Roger Allen https://github.com/rogerallen/raytracinginoneweekendincuda.  <br />

In this version, I use const kernel parameter to store all the scene and cam data.<br />
https://developer.nvidia.com/blog/cuda-12-1-supports-large-kernel-parameters/ <br />
I get around 10x speed up compare to the orignial CUDA RT version.  Const kernel parameters can support 32KB of data <br />
The RT in One weekend scenes use around 20KB. <br />
The number of source code is less the orignial one from Roger Allen because I cut and merge the code here and there to make things work. <br />

This version use CUDA/OpenGL interop to draw the result as a full screen texture quad.
I am also using shader.h from learnopengl.com by Joey de Vries to init some shader codes.

## User guides
use WSAD key to move the camera <br />
drage left mouse to rotate the camera

## Compilation using MSVC 2022 (WIP)
Library used
- GLFW
- glew
- stb_image
- GLM please put it in the includes folder. get it here https://github.com/g-truc/glm
