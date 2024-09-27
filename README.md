# diffdrive_arduino

This ROS 2 Humble package provides a `ros2_control` hardware interface called `DiffDriveArduinoHardware`. It is designed to be used with a `diff_drive_controller` from `ros2_control` and communicates via serial with two motors, each offering velocity control and position/velocity feedback.

## Overview

The package is an adaptation of the original [diffdrive_arduino](https://github.com/joshnewans/diffdrive_arduino/tree/humble) created by Josh Newans. It has been modified to work with the custom firmware developed for my Arduino-based low_level robot controller, available [here](https://github.com/Axelado/my_robot_arduino_ros).

It is expected to communicate over a serial interface, and although primarily designed for Arduino, it could be adapted for other microcontrollers that follow the same communication protocol.

### Key Features

- Hardware interface for two-wheel differential drive robots.
- Serial communication with velocity control and feedback for each motor.
- Compatible with `ros2_control` `diff_drive_controller`.
- Adaptable for different microcontroller platforms.

## Prerequisites

- ROS 2 Humble
- An Arduino (or other microcontroller) flashed with the [custom firmware](https://github.com/Axelado/my_robot_arduino_ros).
- `ros2_control` and `diff_drive_controller` installed.

## Configuration

The package expects a serial communication protocol compatible with the Arduino firmware provided in [my_robot_arduino_ros](https://github.com/Axelado/my_robot_arduino_ros). Ensure your microcontroller firmware adheres to this protocol.

## Contributions

Feel free to contribute or modify the package to suit your specific robot setup. Pull requests and issues are welcome.

## License

This package is licensed under the MIT License.
