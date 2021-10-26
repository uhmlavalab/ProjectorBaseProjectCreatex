# ProjectorBaseProjectCreatex

Aloha! There are a couple of things to keep in mind when developing for the projection system in Create(x)

1- Three camera objects make up the Wall Projector Camera Rig Game Object. Each camera has a script called CAM FOV, this script manipulates the FOV of the
cameras to fix the projectorʻs distortion across the three walls in Create(x). If these varibles are changed, the projections may become warped. Also, this
script may cause problems with shaders that rely on the camera's FOV. 

2- 
Left Wall- Display 2, 
Middle Wall- Display 4, 
Right-Wall Display 5. 

Because of the multiple display set up within Create(x), when any program is built & executed, the cameras's must be set to these target displays, or else
the wrong windows will open on the wrong displays.

3-The Close-Up boundary designates the boundary in which generic Game Objects with a height (scale y) of 1 will fill the entire screen. Anything within
this boundary will be very close to the cameras, so it is suggested to place envrionement elements on the outside of this boundary.

4- If you want to write your own camera controller, remember to take the standard Simple Camera Controller script off of the Wall Camera Rig gameobject.
This script otherwiase controls the movement of the camera rig using a WASD-scheme.

![Alt text](/createxwallexplanation.png?raw=true "Optional Title")
