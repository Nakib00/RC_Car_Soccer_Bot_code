# RC Car and Soccer Bot Control using Bluetooth

This project contains two code variations to control an RC car and a soccer bot using Bluetooth communication. The code is designed to be used with an HC-05 Bluetooth module and a mobile app called "Bluetooth RC car" to send commands from your phone to the Arduino board.

## Folder 1: BTS Motor Driver

### Code Description

This folder contains the Arduino code to control the RC car and soccer bot using the 2 BTS motor driver. The BTS motor driver allows independent control of two DC motors, enabling the robot to move in various directions.

### Wiring

Connect the 2 BTS motor driver to the Arduino board and the motors as described in the circuit diagram provided in the "BTS_Motor_Driver_Circuit.png" file in this folder.

### Usage

1. Upload the code to the Arduino board.
2. Connect the BTS motor driver to the Arduino and the motors as per the circuit diagram.
3. Connect the HC-05 Bluetooth module to the Arduino board.
4. Power on the Arduino and pair the HC-05 Bluetooth module with your phone.
5. Install the "Bluetooth RC car" app on your phone.
6. Open the app, connect to the HC-05 module, and use the on-screen buttons to send commands to control the RC car or soccer bot.

## Folder 2: L298 Motor Driver

### Code Description

This folder contains the Arduino code to control the RC car and soccer bot using the L298 motor driver. The L298 motor driver allows independent control of two DC motors, enabling the robot to move in various directions.

### Wiring

Connect the L298 motor driver to the Arduino board and the motors as described in the circuit diagram provided in the "L298_Motor_Driver_Circuit.png" file in this folder.

### Usage

1. Upload the code to the Arduino board.
2. Connect the L298 motor driver to the Arduino and the motors as per the circuit diagram.
3. Connect the HC-05 Bluetooth module to the Arduino board.
4. Power on the Arduino and pair the HC-05 Bluetooth module with your phone.
5. Install the "Bluetooth RC car" app on your phone.
6. Open the app, connect to the HC-05 module, and use the on-screen buttons to send commands to control the RC car or soccer bot.

## Note

- Make sure to adjust the speed variables (`speed_min` and `speed_max`) in the code to match your motor's specifications.
- Double-check the wiring connections in the circuit diagrams to ensure proper functionality.
- Use the "Bluetooth RC car" app to control the movement of your RC car or soccer bot via Bluetooth from your mobile device.

Enjoy controlling your RC car and soccer bot wirelessly with Bluetooth!

## Circuit Diagrams

### BTS Motor Driver Circuit
![BTS Motor Driver Circuit](https://github.com/Nakib00/RC_Car_Soccer_Bot_code/blob/main/Image/RC%20and%20Soccor%20circuit%20using%202%20BTS.jpg?raw=true)

### L298 Motor Driver Circuit
![L298 Motor Driver Circuit](path_to_l298_motor_driver_circuit.png)

## Usage Instructions

1. **Setup**: Upload the appropriate Arduino code (BTS Motor Driver or L298 Motor Driver) to your Arduino board.

2. **Hardware Connection**:
   - For BTS Motor Driver: Follow the wiring diagram provided in the "BTS_Motor_Driver_Circuit.png" file to connect the 2 BTS motor driver and the HC-05 Bluetooth module to the Arduino board and the motors.
   - For L298 Motor Driver: Refer to the wiring diagram in the "L298_Motor_Driver_Circuit.png" file to connect the L298 motor driver and the HC-05 Bluetooth module to the Arduino board and the motors.

3. **Bluetooth Pairing**: Power on the Arduino board and pair the HC-05 Bluetooth module with your mobile device. Make sure the Bluetooth module is in discoverable mode.

4. **Mobile App**: Install the "Bluetooth RC car" app on your mobile device.

5. **Control**: Open the "Bluetooth RC car" app and connect to the paired HC-05 Bluetooth module.

6. **Control Options**: The app provides on-screen buttons for various directions and actions, such as forward, backward, left, right, etc. Press the buttons to send corresponding commands to the Arduino board.

7. **Adjust Speed**: You can adjust the speed of the motors by changing the `speed_min` and `speed_max` variables in the Arduino code. Experiment with different values to achieve the desired speed for your RC car or soccer bot.

## Notes

- Ensure that the motors are correctly connected to the motor driver outputs.
- The Bluetooth module's baud rate should match the one specified in the Arduino code (9600 in this case).
- For safety, test the movement of the RC car or soccer bot in an open area to avoid collisions or accidents.

Now you have a fully functional RC car and soccer bot that you can control wirelessly using your mobile device! Have fun exploring and experimenting with your robotic creations.
