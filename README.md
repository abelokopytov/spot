# spot
Software for peripheral vision experiments with two smartphones.

Smartphone's display characterization is in the file DisplayCharacterization.xlsx

Both smartphones are Samsung Galaxy S8.
One smartphone is called Checker ("Central") and is placed in the center of the primeter arc,
other smartphone is called Test ("Periph") and can move along the arc (see Fig.1).
Smartphones are in "landscape" mode.

<p align="center">
<img src="https://github.com/abelokopytov/spot/raw/master/figs/fig_1.png" width=50%>
</p>
<p align="center">
Figure 1. General view of the experimental setup.
</p>

The program hsv_40mm_center.html should be opened with web browser (e.g. Chrome) on the Checker smartphone.
This program allows subject to change HSV values with mouse according to Fig.2.
The mouse is attached to the smartphone with OTG dongle.
The program shows stimulus (filled colored circle) at the center of the screen.
Stimulus diameter is 40 mm for Galaxy S8 and can be changed by changing value of the "radius" variable.
Left mouse click initially activate full screen mode, next clicks show/hide numerical HSV values at the top of the screen. 

<p align="center">
<img src="https://github.com/abelokopytov/spot/raw/master/figs/fig_2.png" width=50%>
</p>
<p align="center">
Figure 2. Changing HSV values with mouse
</p>

For foveal matching one should use hsv_40mm_right.html program.
The only difference is the position of the stimulus near the right side of the screen.

Test smartphone is connected to the notebook with WiFi.
Test smertphone's screen is the extension of notebook screen with the help of the SpaceDesk driver (https://spacedesk.net/).
The program spot_rgb.html or spot_hsv.html should be run on the experimenter's notebook.
It's child window then should be moved to the Test smartphone screen and changed to full-screen mode.
In the case of foveal matching experimeter runs variant of the program called spot_rgb_left.html (it shows test stimulus at the left side of the smartphone screen).
The program allows to select primary stimulus color (0 - Red, 1- Green; 2 - Blue), its brightness, start/stop flickering.

For the program to work one need to do 2 things:
1. Allow pop-up windows
2. For Firefox go to about:config and change the parameter
"security.fileuri.strict_origin_policy" to "false"

