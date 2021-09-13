# px4_offb
Offb in python developed for px4 autopilot testing

# Usage
```
mkdir -p ~/workspace/src
cd ~/workspace
catkin_init_workspace
cd src
git clone git@github.com:mamariomiamo/offb_py.git
cd ~/workspace
catkin build
source devel/setup.bash
rosrun px4_offb xxx.py (replace "xxx.py" with the desired node name)
```
## Work with PX4
Launch mavros

```roslaunch mavros px4.launch fcu_url:="udp://:14540@127.0.0.1:14557"```

Launch PX4-SITL

```make px4_sitl gazebo```

Launch Offboard Node

```
cd ~/workspace
source devel/setup.bash
rosrun px4_offb xxx.py (replace "xxx.py" with the desired node name)
```
