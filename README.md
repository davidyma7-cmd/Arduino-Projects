# Arduino-Projects
This is my first arduino project, involving measuring distance of the user in front of the computer screen to protect the eyes.
The Arduino controls an ultrasonic sensor, measuring the distance of the person in front of the screen. If the person is too close for more than 10s, the buzzer will buzz and the LED will light up. When the person become far and in a safe distance for, the buzzing will stop and the LED will get off.
To turn on the function to measure distance and remind the user, the user just need to press the switch once. As the person leaves or becomes very far that the sensor cannot measure (above 5m usually), the sensor will automatically turn-off to save power.
The timing is achieved through using RC charging time with large R and C to delay the turning on time of the NPN switch. The discharging is fast through using a smaller resistor to allow the charges stored in the capacitor to flow to ground fast.
This is the schematic (note: this is just the schematic, even though in reality you need to connect more components like oscillator, switch, or reset, etc for an MCU, but this is just the schematic to demonstrate logic. I am using an education board, which already has all the things wired for the user. NOTE: this version is if the user want to achieve delay by 2 second by hardware): <img width="976" height="635" alt="image" src="https://github.com/user-attachments/assets/315cc015-fda6-4b16-bed3-c782be6f9462" />
This is the version of schematic achieve software delay: <img width="691" height="457" alt="image" src="https://github.com/user-attachments/assets/b98b6ea7-1b97-4a52-820f-285353293819" />
The code on my repo is for software timing only, the user can delete and modify the code if using hardware delay. (note: use hardware delay if your MCU is not a powerful MCU, or an old MCU. Use hardware if your MCU is performing multiple tasks at the same time to minimize the computational resources used for this function.)
This is the physical wiring of the project: <img width="527" height="709" alt="image" src="https://github.com/user-attachments/assets/e9088792-fe5e-4981-8766-4e0b382c79aa" />


