# Introduction

This repo contains code and instructions to run an automated stage repeatability capture on a Nikon system running NIS-Elements. The macro was written by Kees van der Oord of Nikon. 

The function of the macro:

1. Capture an image at the desired FOV.
2. Move 300 um diagonally up and right.
3. Move back to the FOV, capture an image.
4. Continue with the other three diagonals.
5. Wait 30 seconds.
6. Repeat 1-5 twenty times. 
7. Repeat 1-6 but now move 3000 um instead of 300 um.
8. 160 images total.

DISCLAIMER: Any macro which causes automated large movements of the sample has the potential to damage the sample, stage or objectives. Make sure that there is at least 5 um clearance around the selected FOV on the sample slide. This macro has been tested on Elements v xx and xx with stage model xx and is not guaranteed to work with any other versions or models.

# Installation

1. Copy both files to the NIS-Elements macros folder (`C:\Program Files\NIS-Elements\Macros`)	
2. Open NIS-Elements.
3. Select the macro under `Macro | Open`.
4. Open the macro for editing using `Macro | Edit`.
5. Change the stage model and serial number to that of your system.

# Use

1. Turn on the microscope.
2. Choose an air objective.
3. Insert a bead sample (1-4 um in diameter) and ensure it is well secured.
4. Optimise the acquisition settings so that the beads are ~50% of the maximum bit-depth of the microscope detector.
5. Find a suitable bead and centre it in the field of view and focal plane.
6. Run the macro using `Macro | Run`.
