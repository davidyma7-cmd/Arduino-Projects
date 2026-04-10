# Arduino-Projects
This is my first arduino project, involving measuring distance of the user in front of the computer screen to protect the eyes.
The Arduino controls an ultrasonic sensor, meausring the distance of the person in front of the screen. If the person is too close for more than 10s, the buzzer will buzz and the LED will light up. When the person become far and in a safe distance for, the buzzing will stop and the LED will get off.
To turn on the function to measure distance and remind the user, the user just need to press the switch once. As the person leaves or becomes very far that the sensor cannot measure (above 5m usually), the sensor will automatically turn-off to save power.
The timing is achieved through using RC charging time with large R and C to delay the turning on time of the NPN switch. The discharging is fast through using a smaller resistor to allow the charges stored in the capacitor to flow to ground fast.
This is the schematic (note: this is just the schematic, even though in reality you need to connect more components like oscillator, switch, or reset, etc for an MCU, but this is just the schematic to demonstrate logic. I am using an education board, which already has all the things wired for the user.): <img width="1082" height="609" alt="image" src="https://github.com/user-attachments/assets/65d02fea-c55f-4512-8893-bf9ae3ec6682" />
I will upload the code in the future.
This is the physical wiring of the project: <img width="475" height="631" alt="image" src="https://github.com/user-attachments/assets/9240f56b-85b7-48ed-a309-8c289f8b2b78" />

