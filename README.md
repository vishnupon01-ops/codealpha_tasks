# Distance alert system using arduino

# Abstract
	The distance alert system is an Ardiuno-based embedded 
project that measures the distance between an object and an ultrasonic sensor. 
Based on the measured distance, visual alerts are provided using 
LEDs to indicate safe, caution, and danger zones. This project 
demonstrates ultraonic sensing, real-time
monitoring, and conditional decision-making using ardiuno.

# Project Overview
	This system uses an HC-SRO4 ultrasonic distance sensor interfaced 
with an Arduino Uno. The sensor continuosuly measures distance and sends the
data to the ardiuno. The Ardiuno processes this data and activities different 
LEDs according to predefined distance thresholds.

# Components Required
	*Arduino Uno
	*HC-SrO4 Ultrasonic Distance sensor
	*RGB LED
	*Current limiting resistors(220ohm/330ohm)
	*Jumper wires

# Pin Configuration

	Components                    Arduino Pin

	Ultrasonic Trigger Pin        D10
	Ultrasonic Echo Pin           D9
	Green Pin 		      D13
	Blue Pin		      D12
	Red Pin 		      D11

# Working Principle 
	The ultrasonic sensor emits high-frequency sound waves and receives 
the reflected echo from an object. The time taken for the echo to return is used
to calculate the distance between the sensor and the object.

	the calculated distance is continuously compared with predefined limits,
and corresponding LEDs are activated to indicate the distance level.

# Program Logic 
	*The ultranic sensor measures the distance in centimeters.
	*The distance value is displayed on the Serial Monitor.
	*Based on the distance:
		*Green LED glows when the distance is greater than 100cm.
		*Blue LED glows when the distance is between 50 to 100cm.
		*Red LED glows when the distance is less than 50cm.
	*Only one LED is active at any time to ensure clear indication.

# Procedure to Run the Project
	1.connect all component according to the pin configuration table.
	2.Upload the Arduino program to the board.
	3.Open the Serial Monitor.
	4.Place the Serial Monitor.
	5.Observe the LED indication based on the distance.

# Applications
	*Obstacle detection systems.
	*Parking assistance systems.
	*Safety and warning systems.