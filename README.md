# Pulse-rate-monitoring
Pulse rate monitoring system is an easy and reliable IOT system which gives measure of pulse using pulse sensor. The entire system is developed using Arduino and nodeMCU which has inbuilt Wi-Fi module helps in connecting the system to the Blynk Application. Here the pulse rating is measured using Pulse sensor in which the values are observed in Serial monitor and in Blynk App which is a modern IOT application which is operated on web and also available as mobile application. With the help of this system the pulse rate of an individual is easily known.
<br/>The pulse sensor detects the heartbeats and converts them into Analog voltage values.  The Arduino reads these Analog values through the Analog input pin.  The getBPM function can be customized based on the specifications of your pulse sensor. You may need to refer to the sensor datasheet for accurate conversion formulas. The calculated BPM value is sent to the Serial Monitor, where you can observe the pulse rate in beats per minute.

<br/>**Required Hardware components**
<br/>Ardunio UNO, Node MCU, Pulse rate sensor

![image](https://github.com/user-attachments/assets/7ab2f5c9-33cd-403e-9776-8ae9f9f904a5)


<br/>**Methodology and Hardware assembly**
<br/>The whole project is built using the Arduino UNO board. In order to measure the pulse rate the pulse sensor is connected to the Arduino UNO board. The pulse sensor has three pins. The Ground pin is connected to GND and the supply pin of sensor is connected to 5V pin of Arduino UNO. The third pin of sensor is Analog pin which is connected to A0 pin of Arduino board. Whenever the pulse is detected the LED blinks. For that the inbuilt LED of Arduino UNO board is used that is pin number 13 or else it is also possible to connect LED to any of the pin of Arduino on breadboard and resistor (220Ω). Next connect GND and supply pins of nodeMCU to respective 5V and GND pins and connect D6 and D7 pins of nodeMCU to 6th and 7th pins of Arduino. Here we used in built LED which is present on Arduino UNO board. That is pin number 13. As it is not possible to show the inbuilt LED on Arduino the external LED is connected on breadboard.

![image](https://github.com/user-attachments/assets/baf2475b-e7d1-4d66-af7c-19a27113c45b)

<br/>**Results**
<br/> The results are measured in two different ways.
<br/>1. As soon as the finger placed on the sensor, the LED on Arduino blinks and the pulse rate is displayed on the serial monitor.
<br/>2. simultaneously the results are being displayed in Blink App as well.

![image](https://github.com/user-attachments/assets/eebc411f-3b65-41f9-b35b-f9c91381552f)

![image](https://github.com/user-attachments/assets/398488f8-5208-408e-b215-4c2d30cb47fa)

<br/>**NOTE**: Implementing with Blink App is optional.To make it simple, one can implement using simple Arduino UNO board, sensor and observe the desired results on serial monitor. For the implementation using Blink you need Node MCU.




