# spot
Software for peripheral vision experiments with two smartphones.

One smartphone is called Checker and is placed in the center of the primeter arc,
other smartphone is called Test and can move along the arc (see Fig.1). Smartphones are in "landscape" mode.

<p align="center">
<img src="https://github.com/abelokopytov/spot/raw/master/figs/fig_1.png" width=50%>
Figure 1. General view of the experimental setup.
</p>


Both smartphones are Samsung Galaxy S8.

The program hsv_40mm_center.html should be opened with web browser (e.g. Chrome) on the Checker smartphone.
This program allows subject to change HSV values with mouse according to Fig.2.
The mouse is attached to the smartphone with OTG dongle.
The program shows stimulus (filled colored circle) at the center of the screen.
Stimulus diameter is 40 mm for Galaxy S8 and can be changed by changing value of the "radius" variable.
Left mouse click initially activate full screen mode, next clicks show/hide numerical HSV values at the top of the screen. 

<p align="center">
<img src="https://github.com/abelokopytov/spot/raw/master/figs/fig_2.png" width=50%>

Figure 2. Changing HSV values with mouse
</p>

For foveal matching one should use hsv_40mm_right.html program.
The only difference is the position of the stimulus near the right side of the screen.

Test smartphone is connected to the notebook with WiFi.
Test smertphone's screen is the extension of notebook screen with the help of the SpaceDesk driver (https://spacedesk.net/).
The program spot4_4cm.html shoulf be run on the experimenter's notebook.
Its child window then should be moved to the Test smertphone screen and changed to full-screen mode.
In the case of foveal matching experimeter runs program variant spot4_4cm_left.html (it shows test stimulus at the left side of the smartphone screen).
The program allows to select primary stimulus color (0 - Red, 1- Green; 2 - Blue), its brightness, start/stop flickering.
