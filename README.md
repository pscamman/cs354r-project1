# cs354r-project1
### Instructions
To run from executable:  ./Prebuilt
To run from source code: ./buildit && ./Project1

### Description
For this project I started with the buildit/makeit setup linked to in the project description. I found some tutorials to create walls and balls, which is done in the createScene() method in TutorialApplication.cpp. In BaseApplication.h I have a wrapper class for the balls (which are scene nodes/entities as far as ogre is concerned) called Sphere, and then another class called Spheres that has a vector of Sphere. It is told to update (move balls and handle collisions) by ogre's FrameRenderingQueued() method in BaseApplication.cpp. The balls do start at a random speed and in a random direction. The camera can be moved with WASD and turned with the mouse. The initial view is external but all 6 walls exist.

## Extra Credit
### Pysics
The movement of the balls is done with some hand written pseudo-physics of mine, where there is collision with walls and other balls, gravity, loss of energy on surface collision, and some friction when rolling on the ground. They eventually come to rest. Very occasionally two balls will stick to each other, but easily become unstuck when a third ball intervenes.

### Graphics
I enabled shadows, have ambient lighting, and two diffuse lights.