# mirs2502_standard

起動コマンド

source install/setup.bash

ros2 launch mirs mirs.launch.py serial_port:=/dev/ttyUSB1 lidar_port:=/dev/ttyUSB0

ttyUSB以下の数字は状況に応じて変更


モータに速度司令のみ送る場合

ros2 topic pub --once /cmd_vel geometry_msgs/msg/Twist "{linear: {x: 0.5, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 1.0}}"

