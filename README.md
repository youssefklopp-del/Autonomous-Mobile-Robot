# MCT443s Autonomous Mobile Robot

Team workspace for the MCT443s Design of Autonomous Systems project.

**Visibility: PRIVATE until submission.** Keep project files, results, and reports private; any later visibility change requires the owner's explicit decision.

## Team assignments

| Member | Responsibility |
| --- | --- |
| Ahmed Tamer | Mechanical design |
| Islam and Hend | Electrical design and integration |
| Basyouni | Low-level control and ROS2/Gazebo infrastructure |
| Makarios | High-level control and ROS2 navigation |
| Youssef | Standalone MATLAB simulation |
| Bola and Michael | Computer vision |

## Project structure

```text
mechanical/           CAD, chassis, drivetrain, drawings, BOM
electrical/          Schematics, PCB, wiring, power and interfaces
low_level_control/   Firmware, motor control, encoders and embedded interfaces
high_level_control/  Planning, mission logic, navigation algorithms
computer_vision/     Perception, calibration and evaluation
ros2/
  gazebo/            Simulation integration and robot models
  worlds/            Gazebo environments
  launch/            ROS2 launch files
  packages/          ROS2 package source
matlab_simulation/   Independent MATLAB models and experiments
hardware_tests/      Bench tests, procedures and measured results
docs/                Requirements, interfaces, decisions and reports
```

## Parallel simulation workflow

- Basyouni maintains ROS2/Gazebo infrastructure and low-level interfaces; Makarios develops navigation and high-level behavior.
- Youssef develops and runs MATLAB simulation independently. MATLAB must not require ROS2, Gazebo, or a running robot.
- Share documented robot parameters, coordinate frames, units, test scenarios, and result formats so both simulation tracks can be compared.
- Mechanical, electrical, and vision work can progress in parallel using agreed interface contracts in `docs/`.

## Getting started

1. Clone this private repository using your authorized GitHub account.
2. Read your area README and document dependencies before adding implementation.
3. Create a feature branch and open a pull request with a short explanation and relevant validation.
4. Keep source files and reproducible configuration in Git. Exclude credentials, build outputs, large recordings, and generated artifacts.

## Initial status

This is a project scaffold. No working robot, firmware, ROS2 packages, Gazebo worlds, MATLAB model, or vision pipeline is claimed yet. Select and record compatible tool versions, hardware, parameters, and acceptance criteria before implementation.
