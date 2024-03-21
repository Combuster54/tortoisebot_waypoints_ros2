# Testing ros2 waypoints

## Clone this repo inside ros2_ws/src

```
cd ~/ros2_ws/src
git clone https://github.com/Combuster54/tortoisebot_waypoints_ros2 tortoisebot_waypoints
```

## build ros2_ws

```
cd ~/ros2_ws/ && colcon build --packages-select tortoisebot_waypoints && source devel/setup.bash
```

## Start your simulation enviroment

```
ros2 launch tortoisebot_waypoints tortoisebot_waypoints.launch.py
```
## Success test
```
cd ~/ros2_ws
colcon test --packages-select tortoisebot_waypoints --event-handler=console_direct+
```
## print result
```
colcon test-result --verbose
```
## Failed test
```
