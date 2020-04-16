## **ENPM809B: Building a Manufacturing Robot Software System: RWA-2**

This is README to run the ROS package created for group-assignment RWA2. 

Group Members:
1.  An Li
2.  Andre 
3.  Nakul Patel
4.  Revati Naik
5.  Sarvesh Thakur
6.  Srujan Panuganti


## **Package Name: group7_rwa2**
This package consists of a listener (ROS Subscriber) to get the sensor/camera data from the Ariac environment on the screen, and display the sensor/camera readings using various levels of Logging in ROS(We have used ROS_INFO_STREAM in this package). 


## **Minimum System Requirements**
  * ROS Melodic 
  * Gazebo >= 9.6.0 
  * Ariac 2019
  * Ubuntu Desktop 18.04 Bionic (64-bit)


## **Instructions to RUN the package**
1. Create and build a catkin workspace

      `mkdir -p ~/catkin_ws/src`
       
      `cd ~/catkin_ws/`

2.  Extract the package in Catkin Workspace

      `cd ~/catkin_ws/src/group7_rwa2`
         
3. Source the setup.bash to add environment variables to your path to allow ROS to function

      `source /opt/ros/melodic/setup.bash`

4. Build your catkin workspace

      `cd ~/catkin_ws`
       
      `catkin_make`

    Note: Always call `catkin_make` in the root of your catkin workspace. 

5. Overlay your cactkin workspace on top of your environment.

     `cd ~/catkin_ws`

     `source devel/setup.bash`
 
## **Launch the Package**

To run the environment and the listener node, open another terminal and run the following command

     `cd ~/catkin_ws`

     `source devel/setup.bash`

     `roslaunch group7_rwa2 group7_rwa2.launch`
