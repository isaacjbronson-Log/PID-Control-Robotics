# Understanding PID Control

## What is PID?

PID stands for Proportional-Integral-Derivative. It is a feedback control system used to improve precision and stability in mechanical and electronic systems.

PID can be applied to systems such as robotic drivetrains, robotic arms, and drones.

When working with a VEX V5 robot, the inertial sensor can provide heading measurements that allow the controller to determine how far the robot is from its target angle.

A basic PID controller uses several important variables:

- **Current Error:** The difference between the target value and the measured value.
- **Integral:** The accumulated error over time.
- **Previous Error:** The error from the previous calculation.
- **Change in Time:** The time elapsed between calculations.
- **Control Output:** The calculated response sent to the system.

## Understanding the Three Components

### Proportional (kP)
Determines how strongly the controller responds to the current error. A larger proportional response generally produces a stronger correction.

### Integral (kI)
Accumulates error over time. It helps correct persistent errors that proportional control alone may not eliminate.

### Derivative (kD)
Measures how quickly the error is changing. It helps reduce overshoot and oscillation by responding to rapid changes in error.

## PID Formula

The control output is calculated using the three components:

output = (kP × Error) + (kI × Integral) + (kD × Derivative)

Where:

Integral = accumulated error over time

Derivative = change in error / change in time
