Aloha! 
There are a couple of things to keep in mind when developing for the projection system in Create(x)

1- The three cameras that make up the entire projection have a script called CAM FOV, this manipulates the FOV of the cameras
This may cause problems with shaders that rely on the camera's FOV. If these varibles are changed, then the projections may 
be warped.

2- Left- Display 2, Middle- Display 4, Right- Display 5. Because of the computer set up, when any program is built, the cam's
must be set to these target displays, else the wrong windows will open on the wrong displays. 

3-The Close-Up boundary is the limit in which you do not want to have object get any closer to the camera. The Middle ground 
bounds designates the sweet spot between itself and the close-up bounds that is the sweet spot for placing objets in the scene.
However the camera's clipping planes are set to the standard 1000, so you can see objects past this boundary. 

4- If you want to write your own camera controller, remember to take the standard Simple Camera Controller script off of the 
Camera Rig. This controller controls the rig through WASD. 