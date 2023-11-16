# ros2_navbot

## Dependencies

```
Cartographer (Include ROS Package)
Navigation2
Rviz2
```

## Install

```
mkdir bot_ws
cd bot_ws
git clone https://github.com/xerathyang/ros2_navbot.git
```

## Build

```
cd ~/bot_ws
colcon build
source install/setup.bash
```

## Launch

![LaunchStructure](https://i.imgur.com/OEfWu5B.png)

### Cartographer Launch

**!Important: Set use_sim_time to True for Simulation Environment**

```
ros2 launch bot_carto bot_carto.launch.py use_sim_time:=False
```

### Navigation Launch

**!Important: Set use_sim_time to True for Simulation Environment**

```
ros2 launch bot_nav2 bot_nav2.launch.py use_sim_time:=False
```

## Reference

Turtlebot3:
[https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/]

Cartographer ROS:
[https://google-cartographer-ros.readthedocs.io/en/latest/]

Nav2:
[https://navigation.ros.org/]
