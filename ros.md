
##配置ROS系统流程

参考网址`http://wiki.ros.org/jade/Installation/Ubuntu`

* 1.setup source list:`sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`
![first](https://github.com/ChenWenchen/ES2016_14353033/blob/master/image/ros_1.png)

* 2.Make sure Debian package index is up-to-date:`sudo apt-get update`

`sudo apt-get install ros-jade-desktop-full`
![second](https://github.com/ChenWenchen/ES2016_14353033/blob/master/image/ros_2.png)

* 3.rosdep update`sudo rosdep init`

`rosdep update`
![third](https://github.com/ChenWenchen/ES2016_14353033/blob/master/image/ros_3.png)

* 4.Environment setup`echo "source /opt/ros/jade/setup.bash" >> ~/.bashrc
source ~/.bashrc`

`source /opt/ros/jade/setup.bash`

`sudo apt-get install python-rosinstall`

