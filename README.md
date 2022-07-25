# install-the-arm-package
task 3
3-	rosdep update
4-	
5-	sudo apt-get install ros-noetic-catkin
6-	
7-	mkdir -p ~/catkin_ws/src
8-	
9-	cd ~/catkin_ws/
10-	
11-	catkin_make
12-	
13-	cd ~/catkin_ws/src
14-	
15-	git clone https://github.com/smart-methods/arduino_robot_arm.git 
16-	
17-	cd ~/catkin_ws
18-	
19-	rosdep install --from-paths src --ignore-src -r -y
20-	
21-	sudo apt-get install ros-kinetic-moveit
22-	
23-	sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui
24-	
25-	sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher
26-	
27-	sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control
28-	
29-	sudo nano ~/.bashrc
30-	
31-	at the end of the (bashrc) file add the follwing line
32-	(source /home/اسم النظام/catkin_ws/devel/setup.bash)
33-	then 
34-	ctrl + o
35-	
36-	source ~/.bashrc
37-	
38-	roslaunch robot_arm_pkg check_motors.launch
look at the image
![image](https://user-images.githubusercontent.com/109861531/180672872-a37ecd95-0434-4bf9-b60c-fe93f13dee8f.png)

مت
م
