# This is a fork of https://github.com/ajaymin28/Aruco_python
We are using this to calibrate scenes with multiple robots for https://github.com/armaanhammer/ECE-510-Monkey-and-Banana


-----
# Original README:

This is Aruco built in Python using python bindings of opencv.

- Requirements

1. python 3.x
2. opencv 3.x 
3. opencv_contrib (for aruco)


- Packages requirements for python & opencv
install it using pip commands.

1. imutils
2. yaml


I have used anaconda 4 with python version 3.x in windows 7.

- main.py

-> this file contains the main code which loads the 3d object in program, also initializes your camera and finds aruco marker and places the 3d object above the aruco marker.

- objloader.py

-> this file is provided by pygame
refer to www.pygame.org/wiki/OBJFileLoader

- Obj and Mtl files.

obj file is generally created by blender or any 3d object creator program. (gaming softwares)
Mtl is material for the Obj file. (must require or your object will be rendered as black)

- How to use this.

Make sure you calibrate your camera first from calibration directory. (main.py from calibration includes comments to understand)
the generated .yaml file should be used in main.py 

- Calibration

In Aruco_python calibration can be done two ways.

1.using chess board.
2.using aruco board.

I prefer using chess board (refer main method in calibaration/aruco.py)/
-> rename the yaml file to the same name as main directory yaml file (must).

for calibrating using aruco (refer calibration/main.py)

Once it says calibration done and data written in file.
Copy the calibrated yaml file to the main directory and replace the older file (must).

now just run the main.py

->make sure you put all files in one directory.


- How to modify and use other 3d objects.

Requirements

You need to have following

1. Brain (must require)
2. python opengl (an introduction to opengl, and how it works. )
3. blender (to modify and to create new objects as per your requirements.)
4. unity 3d (optional)
5. Aruco marker printed. (http://terpconnect.umd.edu/~jwelsh12/enes100/markergen.html)


visit https://free3d.com/3d-models/obj-file

Download any .obj file that you might require.
Make sure you download obj file that have mtl file with it or only obj file will render black obj on your screen.



Bugs

1. Light is little low on opengl window as compared to opencv window. (make sure you work in environment which have enough light)

Anything you find let me know. :)



- Licence

I do not own any of the obj files, please read the readme file model/zip/sinband directory.

Refernces

1. https://www.uco.es/investiga/grupos/ava/node/26
2. https://rdmilligan.wordpress.com/2015/10/15/augmented-reality-using-opencv-opengl-and-blender/
3. http://jevois.org/moddoc/DemoArUco/modinfo.html


