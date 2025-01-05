# Bottle Plotter

## Mini-project for plotting with GCode onto glass bottles

For a while now I have been bottling beer into soda water glass bottles that are common in south east asia and this project just writes some labels to the bottles.

The design is based on how 3d printers are normally contructed with inspiration from egg plotters, utilising 2020 extrusions for the main frame.

The finished effect with a painted marker gives a hand-designed look to the finished product:

![bottle with plotted text](img/Output.jpg?raw=true|width=200)

- The CAD Design can be viewed / forked here: https://cad.onshape.com/documents/f823072732dbdd75a5273435/w/e640f1ab075ef8e8c9c9e7b2/e/68b6cb054995657771d060c9

![CAD picture 1](img/CAD1.jpg?raw=true|width=100)
![CAD picture 2](img/CAD2.jpg?raw=true|width=200)
![CAD picture 3](img/CAD3.jpg?raw=true|width=200)

- After print in PETG and assembly:
![3d printed 1](img/3D1.jpg?raw=true|width=200)
![3d printed 2](img/3D2.jpg?raw=true|width=200)
![3d printed 3](img/3D3.jpg?raw=true|width=200)
![3d printed 4](img/3D4.jpg?raw=true|width=200)

- Tools used:
    - Onshape for CAD
    - https://github.com/LenardOng/grbl-servo, forked from https://github.com/vankesteren/grbl-servo/fork, with configuration changes
    - https://github.com/cncjs/cncjs for sending GCode to the plotter
    - InkScape to create SVGs and GCode
    - Python to custom process the GCode output
    - Arduino for the controller and GRBL host
    - PrusaSlicer for slicing printer files
 
 - Future improvements:
    - Running on 12v makes micro-stepping unreliable at higher sub-divisions, hence it runs quite loud
    - Using a more capable host with faster firmware to run quieter drivers like the TMC2209
    - Process to convert SVGs to GCode is not easy
    - Some areas of the 3d design are not physically stable but got away with this as it is a pen plotter, so overall machine stress is low
