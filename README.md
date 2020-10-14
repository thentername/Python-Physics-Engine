# Python 2D Physics Engine #

This project is a simple 2D Physics Engine made with Python and Pygame.

It may be used to build a game later on, but for now the engine itself is still under development.


![Physics Engine Running](https://github.com/Trevin-S/Python-Physics-Engine/blob/master/readme_images/engineRunning.png)


### Bodies ###

The engine is based off of bodies, shapes with a position and size that can be collided with.

__Static Body VS Kinematic Body__

The __Static Body__ is the base class for all bodies. These bodies cannot move - they are in a fixed position. They have a material type, coefficient of friction and elastic collision energy return value.

The __Kinematic Body__ inherits from the __Static Body__. These bodies can move - They have mass, velocity, acceleration, force, coefficient of friction, gravitational acceleration, air resistance and momentum transfer (with each other)

### What Needs Work? ###

Currently, the momentum transfer is the feature that needs the most work. I can't seem to get it just right, fixing one issue usually causes another. Currently there is an issue with momentum being transferred to the object with lower energy. The applied force is in the opposite direction it should be. The magnitude is OK and the energy of the system is constant (besides friction), so the issue is purely directional.


### Possible Future Features ###

__Body Linking__ - Connect Kinematic Bodies together, share all kinematics. Treated as one body although may be made of several.

__Rotational Motion__ - Center of Gravities of objects will allow for objects to rotate about them. Forces exerted on objects could cause some energy to be converted into rotational intertia of a kinematic body.

__Ramps__ - Angled Static Bodies could interact with Kinematic bodies in interesting ways. Would require Kinematic bodies to be able to rotate. Force would be redirected upon impact with ramps, and frictional forces, normal forces and gravity would allow objects to accelerate down ramps.

__Circular Collision Masks__ - Currently, collision masks of bodies are strictly rectangular. Circular masks would allow for more shapes to collide naturally.
[![Run on Repl.it](https://repl.it/badge/github/Trevin-S/Python-Physics-Engine)](https://repl.it/github/Trevin-S/Python-Physics-Engine)