# Ultrasonic Distance Measurement using Arduino

This project showcases how to use an ultrasonic sensor to measure distances with an Arduino. It utilizes the ArduinoJson library to send distance measurements in JSON format over the serial connection.

## Requirements

- Arduino board
- Ultrasonic sensor (HC-SR04 or similar)
- ArduinoJson library

## How to Use

1. **Hardware Setup:** Connect the trigPin and echoPin of the ultrasonic sensor to the designated pins on your Arduino board.

2. **Library Installation:** Install the `ArduinoJson` library if you haven't already. You can do this using the Arduino Library Manager.

3. **Upload Code:** Copy and paste the provided code (`ultrasonic_distance_measurement.ino`) into your Arduino IDE and upload it to your Arduino board.

4. **Serial Monitor:** Open the Serial Monitor in the Arduino IDE at a baud rate of 9600. You will see distance measurements printed in JSON format.

## Code Explanation

- The code initializes the ultrasonic sensor pins and sets up the serial communication.

- In the loop, it triggers the ultrasonic sensor, measures the duration of the echo, and calculates the distance.

- The distance measurement is then encapsulated in a JSON object using the `ArduinoJson` library.

- If the distance is greater than 400 or less than 2, a specific message is assigned in the JSON object.

- The JSON object is serialized and sent via the serial connection.

## Example Output
