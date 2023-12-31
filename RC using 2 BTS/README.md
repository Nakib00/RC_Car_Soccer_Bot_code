# RC and Soccer Bot Control using 2BTS Motor Driver

This Arduino code allows you to control an RC and Soccer bot using a 2BTS motor driver. The bot can be controlled via serial communication through a connected device such as a computer or smartphone.

## Prerequisites

To use this code, you will need the following components:

- Arduino board (e.g., Arduino Uno)
- 2BTS motor driver
- DC motors for left and right wheels
- A device with a serial terminal (e.g., computer, smartphone) to send commands

## Wiring

Make the following connections between the Arduino board and the 2BTS motor driver:

- Connect left motor enable (L_EN_FOR_ONE) and right motor enable (R_EN_FOR_ONE) pins to digital output pins on the Arduino.
- Connect left motor PWM (L_PWM_FOR_ONE) and right motor PWM (R_PWM_FOR_ONE) pins to PWM-capable digital output pins on the Arduino.
- Connect left motor enable (L_EN_FOR_TWO) and right motor enable (R_EN_FOR_TWO) pins to other digital output pins on the Arduino.
- Connect left motor PWM (L_PWM_FOR_TWO) and right motor PWM (R_PWM_FOR_TWO) pins to other PWM-capable digital output pins on the Arduino.

Also, connect the motors to the respective output pins on the 2BTS motor driver.

## Usage

1. Upload the code to the Arduino board.
2. Connect the Arduino board to the 2BTS motor driver and DC motors.
3. Connect the Arduino board to a device (e.g., computer) using a USB cable for serial communication.
4. Open a serial terminal on the connected device.
5. Send the following commands through the serial terminal to control the bot:
   - 'F': Move the bot forward
   - 'B': Move the bot backward
   - 'R': Rotate the bot right
   - 'L': Rotate the bot left
   - 'S': Stop the bot

You can also adjust the speed of the bot using the commands '1' to '9', where '1' is the slowest speed and '9' is the highest speed. The command 'q' sets the speed to maximum.

## Note

- Make sure to adjust the `speed_min` and `speed_max` variables according to your motor's specifications.
- Modify the pin numbers in the code to match your actual wiring configuration.

Enjoy controlling your RC and Soccer bot with this 2BTS motor driver control code!