Members Name:
Sabir Ali 232386
Syed Muhammad Askari 232386

Circuit Documentation Summary:
This circuit is designed to control a mobile robot equipped with two hobby gearmotors, an ultrasonic sensor for distance measurement, a servo motor for directional sensing, and an Arduino UNO microcontroller for logic control. The robot can move forwards and backwards, and it can turn left or right based on the distance readings from the ultrasonic sensor. The L298N motor driver is used to drive the gearmotors, and power is supplied by a 9V battery and a 4 x AAA battery mount. The circuit includes toggle and rocker switches for power control.

Component List:
Tower Pro SG90 Servo

Description: A small and lightweight servo motor for precision control.
Pins: Signal, +5V, GND
HC-SR04 Ultrasonic Sensor

Description: An ultrasonic distance sensor capable of measuring distances by emitting and receiving ultrasonic waves.
Pins: VCC, TRIG, ECHO, GND
Toggle Switch SPST

Description: A single-pole single-throw (SPST) toggle switch used to control power to the Arduino UNO.
Pins: L1, COM
9V Battery

Description: A standard 9V battery providing power to the Arduino UNO.
Pins: -, +
Arduino UNO

Description: A microcontroller board based on the ATmega328P, used for controlling the logic of the robot.
Pins: Various digital and analog I/O pins
Rocker Switch

Description: A switch used to control power to the L298N motor driver.
Pins: Output, Input
Hobby Gearmotor with 48:1 Gearbox (Two Instances)

Description: A DC motor with a gearbox used for driving the wheels of the robot.
Pins: Pin 1, Pin 2
L298N DC Motor Driver

Description: A dual H-bridge motor driver capable of driving two DC motors.
Pins: OUT1, OUT2, OUT3, OUT4, 12V, GND, 5V, ENA, IN1, IN2, IN3, IN4, ENB
4 x AAA Battery Mount

Description: A battery mount for four AAA batteries, providing power to the motor driver and servo motor.
Pins: -, +
Wiring Details:
Tower Pro SG90 Servo
Signal: Connected to Arduino UNO D11
+5V: Connected to Arduino UNO 5V
GND: Shared ground with Arduino UNO and HC-SR04 Ultrasonic Sensor
HC-SR04 Ultrasonic Sensor
VCC: Connected to Arduino UNO 5V
TRIG: Connected to Arduino UNO A1
ECHO: Connected to Arduino UNO A2
GND: Shared ground with Arduino UNO and Tower Pro SG90 Servo
Toggle Switch SPST
L1: Connected to 9V Battery +
COM: Connected to Arduino UNO Vin
9V Battery
-: Connected to Arduino UNO GND
+: Connected to Toggle Switch SPST L1
Arduino UNO
GND: Shared ground with L298N DC motor driver, 4 x AAA Battery Mount, HC-SR04 Ultrasonic Sensor, and Tower Pro SG90 Servo
5V: Connected to HC-SR04 Ultrasonic Sensor VCC and Tower Pro SG90 Servo +5V
Vin: Connected to Toggle Switch SPST COM
D5: Connected to L298N DC motor driver IN1
D4: Connected to L298N DC motor driver IN2
D3: Connected to L298N DC motor driver IN3
D2: Connected to L298N DC motor driver IN4
A1: Connected to HC-SR04 Ultrasonic Sensor TRIG
A2: Connected to HC-SR04 Ultrasonic Sensor ECHO
D11: Connected to Tower Pro SG90 Servo Signal
Rocker Switch
Output: Connected to 4 x AAA Battery Mount +
Input: Connected to L298N DC motor driver 12V
Hobby Gearmotor with 48:1 Gearbox (First Instance)
Pin 1: Connected to L298N DC motor driver OUT2
Pin 2: Connected to L298N DC motor driver OUT1
Hobby Gearmotor with 48:1 Gearbox (Second Instance)
Pin 1: Connected to L298N DC motor driver OUT3
Pin 2: Connected to L298N DC motor driver OUT4
L298N DC Motor Driver
OUT1, OUT2: Connected to the first Hobby Gearmotor
OUT3, OUT4: Connected to the second Hobby Gearmotor
12V: Connected to Rocker Switch Input
GND: Shared ground with Arduino UNO and 4 x AAA Battery Mount
IN1: Connected to Arduino UNO D5
IN2: Connected to Arduino UNO D4
IN3: Connected to Arduino UNO D3
IN4: Connected to Arduino UNO D2
4 x AAA Battery Mount
-: Shared ground with L298N DC motor driver and Arduino UNO
+: Connected to Rocker Switch Output
