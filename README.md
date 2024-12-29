# Arduino-4-LED-blink-project
# Arduino 4 LED Blink Project

## Overview
This project demonstrates how to make 4 LEDs blink in sequence using an Arduino Uno. It's perfect for beginners who want to learn basic LED control and sequential blinking.

---

## Components
| **Component**      | **Quantity** | **Description**                              |
|---------------------|--------------|----------------------------------------------|
| Arduino Uno         | 1            | Microcontroller board                        |
| LEDs                | 4            | Any colour (Red, Green, Yellow, etc.)        |
| Resistors (220Ω/330Ω)| 4           | Current-limiting resistors for LEDs          |
| Breadboard          | 1            | For organizing connections                   |
| Jumper Wires        | Several      | For connecting components                    |

---

## Connections
| **Arduino Pin**   | **Component**          | **Connection**                              |
|--------------------|------------------------|---------------------------------------------|
| Pin 8             | LED 1 Anode (+)        | Through a resistor to LED 1                |
| Pin 9             | LED 2 Anode (+)        | Through a resistor to LED 2                |
| Pin 10            | LED 3 Anode (+)        | Through a resistor to LED 3                |
| Pin 11            | LED 4 Anode (+)        | Through a resistor to LED 4                |
| GND               | LED Cathodes (-)       | All LED cathodes connected to GND via resistors |

---

## Arduino Code

Here’s the code to make the 4 LEDs blink in sequence:

```cpp
// Define LED pins
#define LED1 8
#define LED2 9
#define LED3 10
#define LED4 11

void setup() {
  // Set LED pins as output
  pinMode(LED1, OUTPUT);
  pinMode(LED2, OUTPUT);
  pinMode(LED3, OUTPUT);
  pinMode(LED4, OUTPUT);
}

void loop() {
  // Blink LEDs in sequence
  digitalWrite(LED1, HIGH); // Turn LED 1 on
  delay(500);               // Wait for 500 ms
  digitalWrite(LED1, LOW);  // Turn LED 1 off

  digitalWrite(LED2, HIGH); // Turn LED 2 on
  delay(500);               // Wait for 500 ms
  digitalWrite(LED2, LOW);  // Turn LED 2 off

  digitalWrite(LED3, HIGH); // Turn LED 3 on
  delay(500);               // Wait for 500 ms
  digitalWrite(LED3, LOW);  // Turn LED 3 off

  digitalWrite(LED4, HIGH); // Turn LED 4 on
  delay(500);               // Wait for 500 ms
  digitalWrite(LED4, LOW);  // Turn LED 4 off
}

YouTube video on the Arduino 4 LED blink project
“Before we begin, here’s what you’ll need for this project:
An Arduino Uno
4 LEDs (any colour)
4 Resistors (220 ohms or 330 ohms)
Jumper Wires
A Breadboard
And of course, your computer with the Arduino IDE installed.”
We’ll connect:
LED 1 to Pin 8
LED 2 to Pin 9
LED 3 to Pin 10
LED 4 to Pin 11
Then, attach resistors to the negative side of each LED and connect them to the GND pin on the Arduino. This setup ensures that our LEDs won’t burn out.”
“Now it’s time to write the code. Open the Arduino IDE and let’s type in a simple code to make all 4 LEDs blink in sequence.”
