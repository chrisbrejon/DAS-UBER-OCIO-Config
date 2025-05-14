# DAS-UBER-OCIO-Config
Based on my previous configs I have created a minimal OCIO config with different image formations for full CG projects. This is **Color Management** in its most minimalistic and simple form:
* Inputs (textures) are in "linear"
* Rendering and Nuke working space are also in "linear"
* View Transform is for Rec.1886 display

# About the config
* Reference color space is XYZ which is the base of all colourimetry
* All matrixes have been generated using [colour-science](https://www.colour-science.org/apps/) with CAT02
* "linear" stands for "linear_bt.709"
* "cineonlog_rec709" can be used for a matte-painting workflow in Photoshop
* "tlog_egamut" is the shaper space. It can be used for color timing and some log operations (such as sharpen)
* Substance_painter roles were set following [this page](https://mrlixm.github.io/blog/substance-painter-color-management/)
* An inverse of the View Transforms has been provided even though it is not perfect
* One may easily add several colorspaces or displays for HDR output if needed (such as "p3_d65_pq")

# Specificities
* I have added more colorspaces than my previous configs if you want to work in a wide gamut such as P3 or BT.2020
* I recommend image formations that do not break visual cognition such as OpenDRT 1.0.0, JP High Contrast and JP2499
* The ACES 1.0 and 2.0 Output Transforms have only be added for comparison

# Looks
* So far only one look has been added: "Red Look"
* It is meant to be used with the RED IPP2 View Transform
* It has been generated using [Jed Smith's tools](https://github.com/jedypod/open-display-transform/tree/main/look-transforms)
