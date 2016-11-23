# crawler_robot
A crawler robot model equipped flipper arms and its plugin and controller program for gazebo.

## How to build the robot's plugin and controller program with message for controlling flippers.
    $ mkdir build  
    $ cmake ../  
    $ make  

## How to use the robot.
You need two terminals.

At Terminal 1 :  
    $ source setup.bash  
    $ gazebo  

At Terminal 2 :  
    $ cd build  
    $ ./robot_teleop crawler_robot 1  

## About robot\_teleop
The robot control program "robot\_teleop" needs an own name of the robot in gazebo. You can find the own name of the robot in the tree of the models.  
And the program needs the robot's drive type in number. In this case, 1 means differential drive, 2 means skid steer drive. The crawler robot uses differential drive, then you should use 1 as type of drive for the robot.

#### UPDATED 2016.11.24
