setting:
1. connect the uLCD to the mbed
2. open screen on terminal
3. LED1 represents the execution of GestureUI
4. LED2 represents the finish of GestureUI
5. LED3 represents the execution of TILT

GestureUI:
1. use "/GestureUI/run 1" to start the GestureUI function
2. LED1 turn on
3. use gesture to increase or decrease the angle on the uLCD (ring for increasing, slope for decreasing, negative for reseting)
4. press the "user botton" to confirm the angle
5. LED1 turn off

TILT:
1. use "/TILT/run 1" to start the TILT function
2. LED2 turn on
3. put the mbed on the table, LED2 will turn off and LED3 will turn on
4. start to tilt the mbed, if the current_angle(will be showed on uLCD) is more than the angle, then the python will show the event
5. if there is 10 times that the current_angle is more than the angle, python will send the commant to stop this mode 

Result:
![擷取](https://user-images.githubusercontent.com/79572143/117811930-b87bf480-b293-11eb-955a-c9a3c7569567.PNG)
1. connecting to the wifi
![S__30834742](https://user-images.githubusercontent.com/79572143/117812057-e5300c00-b293-11eb-82d3-16c539dbebcd.jpg)
2. select uLCD angle
3. Press USER_BUTTON to confirm angle
4. Start tilt detection mode and Current_angle will show on uLCD
5. tilt over  angle will publish the evet on screen and python will receive it and print it.
6. When over 10 times, python will send the command to stop this mode.
![S__30973956](https://user-images.githubusercontent.com/79572143/118642150-9511f600-b80d-11eb-8eb4-fbdd6303d538.jpg)




