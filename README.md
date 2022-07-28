# install-arduino-robot-arm
mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make

cd ~/catkin_ws/src

git clone https://github.com/Eng-Ruba/arduino_robot_arm.git 

cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y

sudo apt-get install ros-kinetic-moveit

sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control

sudo nano ~/.bashrc

at the end of the (bashrc) file add the follwing line
(source /home/ruba/catkin_ws/devel/setup.bash)
then 
ctrl + o

source ~/.bashrc

roslaunch robot_arm_pkg check_motors.launch
![WhatsApp Image 2022-07-28 at 4 06 09 AM](https://user-images.githubusercontent.com/108241970/181401615-e96041c4-3126-41fc-979a-57a604b701fb.jpeg)


![WhatsApp Image 2022-07-28 at 4 06 08 AM](https://user-images.githubusercontent.com/108241970/181401512-39a9b609-4d86-44c6-b5c8-bddf53b3e7e5.jpeg)

![WhatsApp Image 2022-07-28 at 4 06 08 AM (1)](https://user-images.githubusercontent.com/108241970/181401649-16d0b147-e05b-424b-9bba-80182c872420.jpeg)

