# Project-3-Part-2_A-star-for-Turtlebot

In this project, the A* algorithm is used to drive the path of the turtlebot through a static world. The A_star code plans the path for the bot while the inputs from the user determine the motion set (through angular velocities) and the start and goal point. A ROS node publishes these motions directions to the turtle bot and it executes in the world seen in the following photo:

![image](https://user-images.githubusercontent.com/90218824/164989532-0bf8f017-1552-4728-ae09-594ea0640dd0.png)


In order to run this package, the following needs to be installed on your machine:
    • Ubuntu 16.04/18.04 
    • ROS Kinetic 
    • Gazebo 
    • Turtlebot3 Packages 
    • Python Packages: Numpy, OpenCV-Python, Math, Queue
Get the necessary package from the GitHub repository using the following command:

git clone https://github.com/mturpin331/Project-3-Part-2_A-star-for-Turtlebot.git

Then run the following three commands to configure the workspace

cd ~/catkin_ws
catkin_make
source devel/setup.bash

Once all of that is done, you may run the package by entering the following in the terminal window:

roslaunch searchbot astar.launch  x_pos:=0 y_pos:=4.0 yaw:=3.142

Once the world has opened up, enter a “1” in the terminal window and click enter to prompt the user inputs to come up. Follow the commands for entering the necessary inputs then allow the code to find the path and start executing with the turtlebot (note the x start point should match the x_pos and y_pos entered in the terminal with the roslaunch command). The following is what an output should look like:

![image](https://user-images.githubusercontent.com/90218824/164997195-f6bfa59a-6ffd-4aa7-8fe1-9856a5e2e037.png)

