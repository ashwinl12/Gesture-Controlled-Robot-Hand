# Gesture-Controlled-Robot-Hand

****-- Overview --****
Gesture controlled robot hand is an IoT project which is based on wireless communication, where the data from the hand gestures is transmitted to the robot hand over RF link.
Components
Components used in this project are:
  ->	Arduino
  ->	NRF24L01  RF  modules
  ->	Flex Sensors
  ->	Servo Motors
  ->	Mechanical Hand made out of Cardboard
  ->  Breadboards and jumper wires
  ->	One Glove

#####---- Working----#####

There are two parts of this project:
  1.	Robot Hand ( Which serves as the receiver end of the RF Link )
  2.	Glove ( Which consists of FlexSensors and serves as the transmission end of the RF link)

----- Part1 – The Robot Hand -----

As already mentioned the robot hand serves as the receiver end of the RF link. It is made up of cardboard in a way such that each finger is mechanically movable and imitates human hand gestures. Each and every finger is connected to a servo motor which facilitates the movements of the fingers whenever it rotates. Now, all of these servos are connected to a microcontroller which instructs them to rotate specific degrees at a particular time. An NRF24L01 module is also connected to the Arduino, it receives the radio signals from the other NRF24L01 module and passes it on to the Arduino as analog signals which in turn converts them to digital signals and pass them on as instructions to the servo motors.

----- Part2 – The Glove end -----

The glove part acts as the transmission end of the setup. It consists of Flex sensors, which are nothing but variable resistance strips whose resistance depends on the linearity of the strips, i.e. the more the strip bends the greater the resistance gets. So, as the user bends his/her fingers the resistance varies on the strips and this variation in resistance is sensed by the Arduino and appropriate signal is accordingly sent through the NRF24L01 module to the receiver end.





