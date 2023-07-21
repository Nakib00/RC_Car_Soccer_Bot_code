# Motor Control using L298 Motor Driver

This Arduino code enables you to control two motors using the L298 motor driver. The L298 motor driver allows you to control the speed and direction of two DC motors independently. The code takes input commands from a connected device through serial communication.

## Wiring

Connect the L298 motor driver to the Arduino board and the motors as follows:

**LEFT MOTOR**
- Connect the enable pin (ENA_L) to a digital output pin on the Arduino.
- Connect IN1_L, IN2_L, IN3_L, and IN4_L pins to digital output pins on the Arduino.

**RIGHT MOTOR**
- Connect the enable pin (ENA_R) to another digital output pin on the Arduino.
- Connect IN1_R, IN2_R, IN3_R, and IN4_R pins to other digital output pins on the Arduino.

Also, connect the motors to the respective output pins on the L298 motor driver.

## Usage

1. Upload the code to the Arduino board.
2. Connect the Arduino board to the L298 motor driver and DC motors.
3. Connect the Arduino board to a device (e.g., computer) using a USB cable for serial communication.
4. Open a serial terminal on the connected device.
5. Send the following commands through the serial terminal to control the motors:
   - 'F': Move both motors forward
   - 'B': Move both motors backward
   - 'R': Turn the motors right (rotate right)
   - 'L': Turn the motors left (rotate left)
   - 'S': Stop both motors

You can also adjust the speed of the motors using the commands '1' to '9', where '1' is the slowest speed and '9' is the highest speed. The command 'q' sets the speed to the maximum value.

To make the motors move in diagonal directions, use the commands 'G' (forward-left), 'H' (backward-left), 'I' (forward-right), and 'J' (backward-right).

## Note

- Adjust the `speed_min` and `speed_max` variables according to your motor's specifications.
- Modify the pin numbers in the code to match your actual wiring configuration.

Enjoy controlling your motors with the L298 motor driver!