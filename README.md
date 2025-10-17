# mirs2502_standard
起動コマンド

source install/setup.bash

ros2 launch mirs mirs.launch.py serial_port:=/dev/ttyUSB1 lidar_port:=/dev/ttyUSB0

ttyUSB以下の数字は状況に応じて
