# ArduinoProject

# Introduction

In this workspace I have 8 projects all connected with a smart arduino house...

# Connection 

<img src="/ConnectionDiagram.jpg" alt="Connection" />
<img src="/ConnectionList.jpg" alt="Connection" />

### 1 LED Light

In this project I connected the GND and VCC with G and V on the arduino plus board. The S actually controls the LED light, when S is on HIGH  level it is turned on and when it is on LOW level it is turned off. I made it with delay of 2ms for a blinking effect

### 2: Controlling LED Light

Here I tried to control LED light through a PWM  which is a means of controlling analog output via digital means. It helps control the input voltage between 0V and 5V without changing the resistor constantly..

### 3: Passive Buzzer

Usually for emiting sound we use buzzer whether active or passive. For my project I used passive buzzer firstly to emit fire alarm in the smart house and secondly I made a challenge and tried to emit "do re mi fa so la si do" and at the end I made the "Ode to joy" just for fun. 

### 4: Controlling LED light by pressing button

I made this project based on the previous project just the light is constantly turned on while the press button is pressed and when it is not pressed it is turned off.

### 5:  Motor Servo and controlling window and door

The rotation angle of servo motor is controlled by regulating the duty cycle of PWM (Pulse-Width Modulation) signal. The standard cycle of PWM signal is 20ms (50Hz). Theoretically, the width is distributed between 1ms-2ms, but in fact, it's between 0.5ms-2.5ms. The width corresponds the rotation angle from 0° to 180°. But note that for different brand motor, the same signal may have different rotation angle. //Used literature from Arduino WIKI 

I directly used the Servo function of the Arduino to control the motor. I used digital pins 9 and 10 and I made moving window and door as seen in the video above.

### 6: Fan Module


In this project I used the fan module which controls the rotation direction and spped of the motor. This module is efficient and with high quality fan, which can put out the flame within 20cm distance.


### 7: LCD Display

With I2C communication module, this is a display module that can show 2 lines with 16 characters per line. On the back of LCD display, there is a blue potentiometer for adjusting the backlight. The communication address defaults to 0x27. The original 1602 LCD can start and run with 7 IO ports, but ours is built with Arduino IIC/I2C interface, saving 5 IO ports. Alternatively, the module comes with 4 positioning holes with a diameter of 3mm, which is convenient for you to fix on other devices.

I used this display and connected it with the push button to perform password for opening the door. Also I used to display a message: "Vila Bisera! Welcome" just for fun and to try how it displays the messages.


# NOTE: 

Some of the information about the parts of the houses are used from the official page for Arduino Smart House.
https://wiki.keyestudio.com/Main_Page
