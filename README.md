# Emakefun Micro:bit PH2.0 Sensor:bit Extensions
### [For details, please see the official website](https://emakefun-docs.readthedocs.io/zh_CN/latest/)
# Sensor:bit module introduction
## Basic input module 
### 1. matrix keyboard module
- Initialize matrix keyboard pins SCL, SDO
- ![Matrixkeyboard1.png](sensorbit/Matrixkeyboard1.png)
- Implement Micro:bit to read and display keyboard value
- ![Matrixkeyboard3.png](sensorbit/Matrixkeyboard3.png)
- Sample program
- ![Matrixkeyboard2.png](sensorbit/Matrixkeyboard2.png)
- Use two pins to get the value, hit to display the corresponding letter or number
### 2. Touch button module
- Detect if touched by pin
- ![Touchkeymodule1.png](sensorbit/Touchkeymodule1.png)
- Sample program
- ![Touchkeymodule2.png](sensorbit/Touchkeymodule2.png)
- When the module is touched, it will show a smiley face, otherwise it will show a sad face
### 3. Button Module
- Detect whether the key is pressed by the pin
- ![Keyswitchmodule1.png](sensorbit/Keyswitchmodule1.png)
- Sample program
- ![Keyswitchmodule2.png](sensorbit/Keyswitchmodule2.png)
- When the button is pressed, the smiley emoji will be displayed, otherwise the sad emoticon will be displayed
### 4. Touch the module
- Detect collision by pin
- ![Touchmodule1.png](sensorbit/Touchmodule1.png)
- Sample program
- ![Touchmodule2.png](sensorbit/Touchmodule2.png)
- A happy emoji is displayed when a collision occurs, and a sad emoticon is displayed when it does not occur
### 5. Sliding Rheostat Module
- Get the current resistance value of the varistor (1~100) through the pin
- ![slide resistor1.png](sensorbit/slideresistor1.png)
- Sample program
- ![slide resistor2.png](sensorbit/slideresistor2.png)
- Display the current resistance value of the sliding rheostat, and update the value every second
### 6. Rotary Potentiometer Module
- Get the current voltage value of the rotary potentiometer through the pin
- ![Rotatingpotentiometer1.png](sensorbit/Rotatingpotentiometer1.png)
- Sample program
- ![Rotatingpotentiometer2.png](sensorbit/Rotatingpotentiometer2.png)
- Display the voltage value of the current rotating potentiometer, update the value every second
### 7. Joystick Module
- Initialize pins X, Y, B
- ![Rockermodule1.png](sensorbit/Rockermodule1.png)
- Get analog value via pin X/Y
- ![Rockermodule2.png](sensorbit/Rockermodule2.png)
- Determine if the button is pressed
- ![Rockermodule3.png](sensorbit/Rockermodule3.png)
- Sample program
- ![Rockermodule4.png](sensorbit/Rockermodule4.png)
- When the joystick is pushed up/down/left/right, the LED dot matrix screen will print up/down/left/right patterns. When the joystick is pressed, the LED dot matrix screen will print a happy expression.
### 8. Piano Module V1
- Initialize pins CLK, DIO
- ![Pianomodule11.png](sensorbit/Pianomodule11.png)
- Implement whether to play the piano
- ![Pianomodule12.png](sensorbit/Pianomodule12.png)
- Sample program
- ![Pianomodule13.png](sensorbit/Pianomodule13.png)
- By touching different keys, different music will be generated
### 9. Piano Module V2
- Initialize pins CLK, DIO
- ![Pianomodule21.png](sensorbit/Pianomodule21.png)
- Implement whether to play the piano
- ![Pianomodule22.png](sensorbit/Pianomodule22.png)
- Sample program
- ![Pianomodule23.png](sensorbit/Pianomodule23.png)
- By touching different keys, different music will be generated
### 10. PH2.0 handle
- The PH2.0 handle is connected to the I2C pins by default (ie P19, P20), the following code achieves the effect of PH2.0
- Get controller button state
- ![PH2.0handle1.png](sensorbit/PH2.0handle1.png)
- Get the value of the X/Y axis
- ![PH2.0handle2.png](sensorbit/PH2.0handle2.png)
- Determine if the handle button is released
- ![PH2.0handle3.png](sensorbit/PH2.0handle3.png)
- Determine if the handle button is pressed
- ![PH2.0handle4.png](sensorbit/PH2.0handle4.png)
- Sample program
- ![PH2.0handle5.png](sensorbit/PH2.0handle5.png)
- Get the value of the X/Y axis. After 1 second, the function of judging the state of each button can be realized. If it is pressed, it will display a crying face, and when it is released, it will display a smiling face
## sensor
### 1. Water vapor sensor
- Get the water vapor concentration in the environment through the pin
- ![Watervaporsensor1.png](sensorbit/Watervaporsensor1.png)
- Sample program
- ![Watervaporsensor2.png](sensorbit/Watervaporsensor2.png)
- Display the water vapor concentration value, which is updated every second
### 2. LM35 temperature sensor
- Get ambient temperature through pin
- ![LM35temperaturesensor1.png](sensorbit/LM35temperaturesensor1.png)
- Sample program
- ![LM35temperaturesensor2.png](sensorbit/LM35temperaturesensor2.png)
- Display the ambient temperature value and update the display every second
### 3. Flame sensor
- Judging that there is flame around by the digital value obtained from the pin
- ![Flamesensor1.png](sensorbit/Flamesensor1.png)
- Get the analog value of the flame through the pin
- ![Flamesensor2.png](sensorbit/Flamesensor2.png)
- Sample program
- ![Flamesensor3.png](sensorbit/Flamesensor3.png)
- Judging whether there is a flame around, if there is an analog value to display the flame, if it does not exist, it will display a smiley face.
### 4. Infrared tracking sensor
- Determine if there is a black wire by the pin
- ![Fourwaytrackingsensor1.png](sensorbit/Fourwaytrackingsensor1.png)
- Sample program
- ![Fourwaytrackingsensor2.png](sensorbit/Fourwaytrackingsensor2.png)
- If the infrared tracking sensor senses a black line, it will display a crying face, otherwise it will display a smiling face
### 5. Tilt Sensor
- Judging whether it is tilted by the pin
- ![Inclinationsensor1.png](sensorbit/Inclinationsensor1.png)
- Sample program
- ![Inclinationsensor2.png](sensorbit/Inclinationsensor2.png)
- When the tilt sensor senses tilt, it will show a crying face, otherwise it will show a smiling face
### 6. Light sensor
- Get the analog value of the light intensity sensed by the light sensor in the environment through the pin
- ![Photosensitivesensor1.png](sensorbit/Photosensitivesensor1.png)
- Sample program
- ![Photosensitivesensor2.png](sensorbit/Photosensitivesensor2.png)
- Displays an analog value of light intensity, updating the display every second
### 7. Thermal Sensor
- Get heat value by pin
- ![Heatsensitivesensor1.png](sensorbit/Heatsensitivesensor1.png)
- Sample program
- ![Heatsensitivesensor2.png](sensorbit/Heatsensitivesensor2.png)
- Display the ambient heat value, update the display every second
### 8. Water depth sensor
- Get water depth value via pin
- ![Waterdepthsensor1.png](sensorbit/Waterdepthsensor1.png)
- Sample program
- ![Waterdepthsensor2.png](sensorbit/Waterdepthsensor2.png)
- Display the water depth value, which is updated every second
### 9. Soil Moisture Sensor
- Get soil moisture value via pin
- ![Soilmoisturesensor1.png](sensorbit/Soilmoisturesensor1.png)
- Sample program
- ![Soilmoisturesensor2.png](sensorbit/Soilmoisturesensor2.png)
- Display soil moisture value, update display every second
### 10. Obstacle Avoidance Sensor
- Get the digital value through the pin to determine whether there is an obstacle ahead
- ![Obstacleavoidancesensor1.png](sensorbit/Obstacleavoidancesensor1.png)
    sample program
- ![Obstacleavoidancesensor2.png](sensorbit/Obstacleavoidancesensor2.png)
- Determine whether there is an obstacle in front of you, if there is a crying face, if not, a smiling face is displayed
### 11. Reed switch sensor
- Get the digital value through the pin to determine whether there is a magnetic field around
- ![Reedswitchsensor1.png](sensorbit/Reedswitchsensor1.png)
- Sample program
- ![Reedswitchsensor2.png](sensorbit/Reedswitchsensor2.png)
- The reed switch sensor senses whether there is a magnetic field around it, and if it exists, it will show a sad face, and if it does not exist, it will show a smiling face
### 12. Human body heat sensor
- Realize the function of obtaining the digital value obtained by the human body heat source sensor through the pin, thereby judging whether there is an ambient heat source around
- ![Humanbodyheatsourcesensor1.png](sensorbit/Humanbodyheatsourcesensor1.png)
- Sample program
- ![Humanbodyheatsourcesensor2.png](sensorbit/Humanbodyheatsourcesensor2.png)
- Determine whether there is a human body heat source around, if it exists, it will show a crying face, if not, it will show a smiling face
### 13. Shock Sensor
- The vibration sensor is a 4Pin sensor, the D port connected is used to detect whether vibration (digital value) is detected, and the Pin port connected to the A port is used to read the analog value.
- Get shock sensor analog value via pin
-
