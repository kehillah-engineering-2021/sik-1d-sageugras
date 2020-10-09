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
```
  int photoresistor = A0;          //variable for storing the photoresistor value
  int potentiometer = A1;          //this variable will hold a value based on the position of the knob
  int threshold = 700;            //if the photoresistor reading is lower than this value the light will turn on
```
3. If the light level variable is above the threshold, call the function that turns the RGB LED off.
4. If the light level variable is below the threshold, call one of the color functions to turn the RGB LED on.
```
  if (photoresistor < threshold) {}
  
  else {                                //if it isn't dark turn the LED off

    turnOff();                            //call the turn off function
    }
```
5. If potentiometer is between 0 and 100, turn the RGB LED on color changing mode.
```
    if (potentiometer > 0 && potentiometer <= 100)
      changing();
```
6. If potentiometer is between 100 and 200, turn the RGB LED on green to red fade.
```
    if (potentiometer > 100 && potentiometer <= 200)
      greenred();
```
7. If potentiometer is between 200 and 300, turn the RGB LED on crazycolor1.
```
 if (potentiometer > 200 && potentiometer <= 300)
      crazycolor1();
```
8. If potentiometer is between 300 and 400, turn the RGB LED on orange.
```
if (potentiometer > 300 && potentiometer <= 400)
      orange();
```
9. If potentiometer is between 400 and 500, turn the RGB LED on yellow.
```
 if (potentiometer > 400 && potentiometer <= 500)
      yellow();
```
10. If potentiometer is between 500 and 600, turn the RGB LED on green.
```
    if (potentiometer > 500 && potentiometer <= 600)
      green();
```
11. If potentiometer is between 600 and 700, turn the RGB LED on crazycolor2.
```
    if (potentiometer > 600 && potentiometer <= 700)
      crazycolor2();
```
12. If potentiometer is between 700 and 800, turn the RGB LED on cyan.
```
    if (potentiometer > 700 && potentiometer <= 800)
      cyan();
```
13. If potentiometer is between 800 and 900, turn the RGB LED on blue.
```
  if (potentiometer > 800 && potentiometer <= 900)
      blue();
```
14. If potentiometer is greater than 900, turn the RGB LED on magenta.
```
  if (potentiometer > 900)
      magenta();
```

### Code in Action

![ezgif com-optimize](https://user-images.githubusercontent.com/54454824/95606746-a55c2a00-0a0f-11eb-836e-5d007eefe425.gif)



