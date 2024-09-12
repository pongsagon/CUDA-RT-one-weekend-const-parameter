# CUDA-RT-one-weekend-const-parameter
Modify Ray Tracing in One Weekend by Peter Shirley http://in1weekend.blogspot.com/2016/01/ray-tracing-in-one-weekend.html 
and CUDA code by Roger Allen https://github.com/rogerallen/raytracinginoneweekendincuda.  <br />

In this version, I use const kernel parameter to store all the scene and cam data.<br />
https://developer.nvidia.com/blog/cuda-12-1-supports-large-kernel-parameters/ <br />
I get around 10x speed up compare to the orignial CUDA RT version.  Const kernel parameters can support 32KB of data <br />
The RT in One weekend scenes use around 20KB. <br />

This version use CUDA/OpenGL interop to draw the result as a full screen texture quad.

## User guides
use WSAD key to move the camera <br />
drage left mouse to rotate the camera

## Compilation guides
todo
