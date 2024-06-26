Franya Chandler 1103745 4DOF Manipulator Arm: Design and Simulation 

Below are instructions to using the packages in this repository. 

1. Download and unzip the two packages (myrobot_description and config) into your catkin_ws.
   
   $ catkin_make
   
3. Ensure that the two python programs (myrobot_descripton > scripts) are executable (using chmod +x _____.py)
   
   $ catkin_make
   
5. Simulations Part 1: Launch the demo_gazebo.launch file using the line below:
   
      $ roslaunch config demo_gazebo.launch
   
   Once the launch process is complete, you may observe the robot's movements by using the 'MotionPlanning' in RViz.
   Under Query, you may choose 'random' Start States and Goal States, then Plan and Execute to observe the robot in Gazebo.
   
7. Simulations Part 2: In one terminal tab, launch the gazebo.launch file using the command line below:

     $ roslaunch myrobot_description gazebo.launch

  In another, launch the teleop.launch file using the command line below: 
  
      $ roslaunch myrobot_description teleop.launch
      
  Once the two are launched, you may control the robot using the instructions specified in the teleop.launch terminal. 
