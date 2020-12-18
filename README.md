# 1D-Pendulum-With-Gearbox
Using MATLab to simulate various configurations of an electromechanical system.

## Objective
Control the motion of a pendulum connected to a motor via a gearbox. Different simulations were created with varying degrees of complexity to achieve a more realistic simulation of the control system. The final goal is to determine the appropriate parameters to achieve system stability.   

This is accomplished by using MATLab Simscape to construct each system. 

## Short Description of the Different Simulations
1) Pendulum, electric motor, and neglecting pendulum mass
2) Pendulum, gear box, and replace electric motor with ideal torque source using trapezoidal signal
3) Pendulum, gear box, and replace electric motor with ideal torque source using step signal
4) Pendulum, gear box, and electric motor using trapezoidal signal
5) Pendulum, gear box, replace electric motor with PID controller, and use positional feedback control
6) Pendulum, gear box, replace electric motor with PID controller (with +/- 3 saturation limit), and use positional feedback control
7) Pendulum, gear box, replace electric motor with PID controller (with D=2), and use positional feedback control
8) Pendulum, gear box, replace electric motor with PID controller, use positional feedback control, and add torsional damper
9) Pendulum, gear box, replace electric motor with PID controller, use positional feedback control, and add torsional spring between PID controller and gear box
10) Pendulum, gear box, replace electric motor with PID controller, and use speed feedback control
11) Pendulum, gear box, electric motor, and use positional feedback control

## Initial Conditions
- Pendulum position: 0 degrees
- Pendulum mass: 4 kg
- Pendulum CG location: 0.25 m
- Gravity: 9.81 m/s^2
- Gear ratio: 2
- Motor inertia: 0.0851 kg*m^2
- Shaft inertia: 0.37 kg*m^2
- Resistor: 5 ohm 
- Inductor: 0.04 H
- Voltage Source: 10 V
- Electromechanical converter constant: 0.1 N*m/A 
- PID controller gains:
    - Proportional: 50
    - Integral: 200
    - Derivative: 5