# serial-number-macro
Numeric control program (G-Code) to engrave a four digit serial number based on the macro variables stored. Tested working in simulation and several friends/customers are using it in production.

## Disclaimer
*Applied Engineering & Design, nor Mike Centola, accepts any responsibility for the misue of the techniques shown in this numeric control program. We publish this information because we feel it will be of interest to CNC users, hobbyests and enthusiasts. In all cases, the end user is totally responsible for considering the inmplications, good and bad, of implementing one or more of the techniques shown here.*


## Screenshot
![Screenshot](http://i.imgur.com/oo9iCC8.jpg)

## General Usage
You will want to call the subprogram from you main program using `G65 P5000 A B C I J K D X Y` and your main program should handle the incrementing of the serial number variables. 

## Passed Variables
```
#1 = A = TOOL NUM
#2 = B = FEED RATE
#3 = C = RPM
#4 = I = ENGRAVING DEPTH
#5 = J = LETTER SPACING
#6 = K = SCALE FACTOR = 1.0
#7 = D = CLEARANCE PLANE
#24 = X = START X
#25 = Y = START Y
```


## Global Macro Variables
```
#500 = 1st Digit
#501 = 2nd Digit
#502 = 3rd Digit
#503 = 4th Digit
```


## Variations
Currently the only variation is the one using CAMBAM Stick Font 2 and numbers only. I will be adding other fonts as well as letters for prefixes.


## Contributing
If you would liek to help contribute to the code or this project, feel free to fork it and submit pull requests to help out!


## About Applied Eng & Design
We are a full service engineering and design firm, specializing in CAD/CAM, CNC milling, rapid prototyping, training and more.  We also like to dabble in Arudino / RaspberryPi projects, electronics, drones and robotics projects! Subscribe to our YouTube channel for videos on our projects, screencast tutorials, and more!

## License
This code is licensed under the [GPL v3 license](https://www.gnu.org/licenses/gpl-3.0.en.html).