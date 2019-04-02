# OpenSourceCoconuts-Neon-Sign
Creating files for CNC milling to make Neon-LED signs

# Goal

![](https://github.com/dusjagr/OpenSourceCoconuts-Neon-Sign/raw/master/fish_gaudi_mini-Signs.jpg)

## Testing the dimensions and bending possibilities

![](https://github.com/dusjagr/OpenSourceCoconuts-Neon-Sign/raw/master/Neon-LED-strip_bendingTests.jpg)

## Inkscape tricks for file preparations

To test your design, check for sharp inner corners. There are these options "Inset" and "Outset", which can create a new path further outside or inside. The settings of the spacing ar somewhere deeply hidden in the preferences -> Behaviour -> Steps

Towards the inside, this will lead to sharper corners though and might reach the limit of corners.

![](https://github.com/dusjagr/OpenSourceCoconuts-Neon-Sign/raw/master/inkscape_testBall.png)

But we found a better way with the following plugin (after failed tests with Fillet...)

Extension to make Rounded Corners: https://github.com/hawley577/Inkscape-Rounded-Corners

From our experience above a minimum radius of 4mm was feasible. so for the center line we need to add 9mm/2 = 8.5mm radius to make rounded Corners. If the shape is too small to even fit such a radius, the extension might not work, so just fix your design.

![](https://github.com/dusjagr/OpenSourceCoconuts-Neon-Sign/raw/master/Inkscape_preparation_RoundedCorners.png)

And after this you just set the stroke width to 9mm. And now choose "Stroke to Path" to generate the inner and outer paths for CNC.







