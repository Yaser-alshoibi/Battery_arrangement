# Battery Arrangement

# Consumption Calculation

After calculating current consumption as following:

2x Potentiometer = 0.04 mA

2x LED = 40mA

5x Servo motor = 500mA

Ultrasonic = 30 mA

h-bridge = 200mA

Arduino Uno = 11.4 mA

total current consumption = 770.04 mA

So by using 7.4V 8000 mAh battery our circuit will operate for:

8000/770.04 = 10.4 hours


![Battery](https://user-images.githubusercontent.com/85786699/125369679-6a639a00-e385-11eb-80b4-d9235f1b983c.jpg)


So approximately and without consedring real life losses this battery can run the robot for 10 and a half hours!




# Circuit Connections

By using this connection shown in the picture and replacing the 9V battery and connecting arduino though Vin:

![battery](https://user-images.githubusercontent.com/85786699/125369782-a991eb00-e385-11eb-84df-6e90bd03f2f2.PNG)


- For servo motors they need voltage between 4 to 6.4V and 100mA . So they can be powered from 5V arduino output or by using stepdown transformer connected with the battery.
- For arduino, it can operate between 6V to 20V but it works unstable under 7V and if we supplie it with more than 12V it will cause the internal regulator to overheat so it's recommended to operate between 7V to 12V So we can connect it directly to the battery through Vin pin on arduino
- For the H-bridge it can operate on range from 4.5V to 38V.
- Potentiometers will work through the 5V output from arduino.
- Robot eyes if we used two leds they can be powered through 5V output of the Arduino with resistor to devide voltage.
- Ultrasonic sensor also can work by 5V output of Arduino
