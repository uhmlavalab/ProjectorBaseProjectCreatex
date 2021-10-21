Aloha! There are a couple of things to keep in mind when developing for the projection system in Create(x)

1- The three cameras that make up the entire projection have a script called CAM FOV, this manipulates the FOV of the cameras This may cause problems with shaders that rely on the camera's FOV. If these varibles are changed, the projections may be warped.

2- Left Wall- Display 2, Middle Wall- Display 4, Right-Wall Display 5. Because of the computer set up within Create(x), when any program is built & executed, the cam's must be set to these target displays, or else the wrong windows will open on the wrong displays.

3-The Close-Up boundary is the limit in which you do not want to have objects get any closer to the camera.

4- If you want to write your own camera controller, remember to take the standard Simple Camera Controller script off of the Wall Camera Rig object. This controller controls the rig through WASD.
