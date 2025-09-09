# Simulink Model of a Self-Balancing Robot Using PID Control

## Overview

This project presents a MATLAB Simulink and Simscape Multibody model of a two-wheeled self-balancing robot, designed to function as an inverted pendulum stabilized via a PID feedback controller. The simulation replicates the key dynamics of a self-balancing robot, offering a comprehensive perspective on both control system principles and practical mechanical modeling.

## Key Features

- **3D Mechanical Simulation:**  
  The robot model incorporates three horizontal plates, four vertical rods forming the body, and two actuated wheels. The system is built using Simscape Multibody, with realistic connections, including revolute and prismatic joints, to accurately mimic actual robot mechanics.

- **Inverted Pendulum Problem:**  
  The project addresses the classic challenge of balancing an inherently unstable two-wheeled structure, a common control engineering and robotics problem.

- **PID Control Implementation:**  
  A PID controller continuously senses the pendulum’s tilt and computes a corrective force to the base (cart), maintaining the upright posture. The controller parameters are tuned to minimize oscillations and stabilize the robot against step disturbances.

- **Dynamic Simulation and Output Analysis:**  
  The simulated system experiences real-world-like disturbances. Outputs—including angular position and cart displacement—are tracked and visualized, demonstrating the successful stabilization of the robot after initial tilts.

## Simulation Process

1. The robot starts at rest, and a step input simulates an initial tilt.
2. The pendulum angle is continuously measured and fed back to the controller.
3. The PID controller processes the angular error (between actual and desired angles).
4. A resulting force actuates the cart, moving it to restore balance.
5. The pendulum returns to its vertical position as the system stabilizes within the simulation period.

## Conclusion

This simulation confirms that a PID-controlled self-balancing robot can efficiently maintain stability and respond quickly to disturbances. The control strategy and mechanical design are validated, providing a strong foundation for further research and development in robotics and model-based control systems.
