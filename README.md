# Sik-1D README
## By: sageugras

### Introduction
In this circuit, you'll take the night-light concept to the next level by adding an RGB LED, which is three differently colored Light-Emitting Diodes (LEDs) built into one component. RGB stands for Red, Green and Blue, and these three colors can be combined to create any color of the rainbow!
### How to Run Code
Parts needed:

![1Dparts](https://user-images.githubusercontent.com/54454824/95239577-fc6bc000-07bf-11eb-885f-bb6cd45b84cc.png)

An RGB LED is actually three small LEDs --- one red, one green and one blue --- inside a normal LED housing. The RGB LED included in this kit has all the internal LEDs share the same ground wire, so there are four legs in total. To turn one color on, ensure ground is connected, then power one of the legs just as you would a regular LED. If you turn on more than one color at a time, you will see the colors start to blend together to form a new color.

![RGB_LED_Pins](https://user-images.githubusercontent.com/54454824/95239584-ff66b080-07bf-11eb-8c3b-e289f902548f.png)

Hookup Guide:

![SIK_Circuit_1D-RGBNightlight](https://user-images.githubusercontent.com/54454824/95239588-0097dd80-07c0-11eb-9aff-9289cdac4d06.jpg)

### Code Explanation
1. Store the light level from pin A0 in the variable photoresistor.
2. Store the potentiometer value from pin A1 in the variable potentiometer.
3. If the light level variable is above the threshold, call the function that turns the RGB LED off.
4. If the light level variable is below the threshold, call one of the color functions to turn the RGB LED on.
5. If potentiometer is between 0 and 150, turn the RGB LED on red.
6. If potentiometer is between 151 and 300, turn the RGB LED on orange.
7. If potentiometer is between 301 and 450, turn the RGB LED on yellow.
8. If potentiometer is between 451 and 600, turn the RGB LED on green.
9. If potentiometer is between 601 and 750, turn the RGB LED on cyan.
10. If potentiometer is between 751 and 900, turn the RGB LED on blue.
11. If potentiometer is greater than 900, turn the RGB LED on magenta.

### Code in Action



