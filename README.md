📖 About

This project demonstrates how to measure distance using an HC-SR04 ultrasonic sensor connected to an ESP32.

🧰 Hardware Required

ESP32 Development Board

HC-SR04 Ultrasonic Sensor

Breadboard

Jumper Wires

USB cable

⚙️ How It Works

The ESP32 sends a 10µs pulse through the TRIG pin.
The sensor emits an ultrasonic wave.
When the wave hits an object, it reflects back.
The ECHO pin stays HIGH for the time the wave travels.
The ESP32 measures this time using pulseIn().
Distance is calculated using the speed of sound.

Formula used:

distance = (duration * 0.0343) / 2

Where:

duration = time for the wave to return
0.0343 cm/µs = speed of sound
divided by 2 because the wave travels to the object and back


▶️ Running the Project
Connect the circuit as shown above.
Upload the code to the ESP32 using Arduino IDE.
Open the Serial Monitor.
Set baud rate to 115200.
Move an object in front of the sensor to see distance readings.
