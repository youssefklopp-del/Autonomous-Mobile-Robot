# ROS2 integration

Infrastructure and Gazebo owner: Basyouni. Navigation owner: Makarios.

- gazebo/: robot simulation integration, models and simulator configuration.
- worlds/: simulation environments and test scenarios.
- launch/: system and simulation launch files.
- packages/: ROS2 package source, including navigation integration.

Agree on a compatible ROS2 distribution and Gazebo release, then document dependencies and launch commands. Document frames, topics, message types, QoS, rates, and simulation time in docs. Build from a ROS2 workspace using the agreed package layout.

The matlab_simulation directory is an independent track and must not depend on this workspace. No executable ROS2 packages or launch files exist yet.
