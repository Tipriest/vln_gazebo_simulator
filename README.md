# README.md
hello and welcome

## Install
```bash
git clone -b humble git@github.com:ROBOTIS-GIT/DynamixelSDK.git
```



## Build
```bash
cd ~/turtlebot3_ws/src/
git clone -b humble https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git
cd ~/turtlebot3_ws && colcon build --symlink-install

export TURTLEBOT3_MODEL=burger
ros2 launch turtlebot3_gazebo empty_world.launch.py

export TURTLEBOT3_MODEL=waffle
ros2 launch turtlebot3_gazebo turtlebot3_world.launch.py

export TURTLEBOT3_MODEL=waffle_pi
ros2 launch turtlebot3_gazebo turtlebot3_house.launch.py
ros2 run turtlebot3_teleop teleop_keyboard
```

## Reference
[turtlebot3的官方文档](https://emanual.robotis.com/docs/en/platform/turtlebot3/simulation/#gazebo-simulation)
