SOP to run big chicken:

!!set master on your own computer!!

make sure pi is connected to "ditrobotics_5G"

if pi is connected to "DITROBOTICS_5G",  type command : "rescan" and then "reconnect"
those command should reconnect pi to "ditrobotics_5G", and then reconnect to pi

1. launch lidar and communication on pi:
roslaunch testbot serial.launch

2. launch lidar localization on your own computer:
roslaunch lidar_localization lidar_localization.launch

3. lauch main:
roslaunch main2021 main_goap2020_demo.launch

on gui: choose strategy 4, click prepare, set

and to start type:
rosparam set /start 1# big_chicken
