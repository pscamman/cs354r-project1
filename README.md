# cs354r-project1

For this project I started with the buildit/makeit setup linked to in the project description. I found some tutorials to create walls and balls. I have a wrapper class for the balls (which are scene nodes/entities as far as ogre is concerned) called Sphere, and then another class called Spheres that has a vector of Sphere and is told to update (move balls and handle collisions) by ogre's FrameRenderingQueued method. The balls do start at a random speed and in a random direction. The camera can be moved with WASD and turned with the mouse. The initial view is external but all 6 walls exist.

## Extra Credit
### Pysics
The movement of the balls is done with some hand written pseudo-physics of mine, where there is gravity, loss of energy on surface collision, and some friction when rolling on the ground. They eventually come to rest. Very occasionally two balls will stick to each other but easily become unstuck.

### Graphics
I enabled shadows, have ambient lighting, and two diffuse lights.