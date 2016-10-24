### 安装ROS
**按顺序执行以下指令**  
1.sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'  
2.sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-key 0xB01FA116  
3.sudo apt-get update  
4.sudo apt-get install ros-jade-desktop-full  
5.sudo rosdep init  
6.rosdep update  
7.echo "source /opt/ros/jade/setup.bash" >> ~/.bashrc  
8.source ~/.bashrc  
9.sudo apt-get install python-rosinstall  
