# serial-number-macro

Numeric control program (G-Code) to engrave a four digit serial number based on the macro variables stored. Tested working in simulation and several friends/customers are using it in production.

## Disclaimer

*Applied Engineering & Design, nor Mike Centola, accepts any responsibility for the misue of the techniques shown in this numeric control program. We publish this information because we feel it will be of interest to CNC users, hobbyests and enthusiasts. In all cases, the end user is totally responsible for considering the inmplications, good and bad, of implementing one or more of the techniques shown here.*

## Screenshot

![Screenshot](http://i.imgur.com/oo9iCC8.jpg)

## General Usage

You will want to call the subprogram from you main program using `G65 P5000 A I J K E F R S T X Y Z` and your main program should handle the incrementing of the serial number variables.

## Passed Variables

```gcode
( VARIABLES PASSED )
( #1 = A = SERIAL NUMBER TO ENGRAVE )
( #4 = I = ANGLE OF ROTATION ) **OPTIONAL**
( #5 = J = SCALE FACTOR / TEXT HEIGHT = 1.0 ) **OPTIONAL**
( #5 = K = LETTER SPACING ) **OPTIONAL**
( #8 = E = PLUNGE FEED RATE ) **OPTIONAL**
( #9 = F = ENGRAVING FEED RATE )
( #18 = R = CLEARANCE / RETRACT PLANE )
( #19 = S = SPINDLE RPM )
( #20 = T = TOOL NUM )
( #24 = X = START X )
( #25 = Y = START Y )
( #26 = Z = ENGRAVING DEPTH )
```

## Variations

Currently the only variation is the one using CAMBAM Stick Font 2 and numbers only. I will be adding other fonts as well as letters for prefixes.

## Contributing

If you would liek to help contribute to the code or this project, feel free to fork it and submit pull requests to help out!

## About Applied Eng & Design

We are a full service engineering and design firm, specializing in CAD/CAM, CNC milling, rapid prototyping, training and more.  We also like to dabble in Arudino / RaspberryPi projects, electronics, drones and robotics projects! Subscribe to our YouTube channel for videos on our projects, screencast tutorials, and more!

## License

This code is licensed under the [GPL v3 license](https://www.gnu.org/licenses/gpl-3.0.en.html).
