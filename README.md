# publisher-subscriber-nodes-using-Python
# 2 nodes shared a string message in a custom package on ROS

First : Create a ROS workspace (choose directory to work on it)
I make it inside document

  $ cd ~/Documents 
  $ mkdir sam_ws
  $ cd sam_ws/
  $ mkdir src 
  $ cd src/
  $ katkin_init_workspace
  
  
 - back to your workspace directory to compile it :
  $ catkin_make
  - make sure there are 2 folder builded (build and devel) into the workspace
   
  Second : Create a new package 
 - move to src directory by " $cd src " if you in workspace directory
  $ catkin_create_pkg robot_tutorials rospy roscpp std_msg
 
   - make sure there is a new packge called "robot_tutorials" in src folder
   -make sure this package containe (CMakeLists , include , package.xml and src) by " $ ls /robot_tutorials "
 
 - back to your workspace directory 
  $ catkin_make
 
 
Third : Create publisher & subscriber nodes using Python:

- write the code of publisher and subscriber codes in text file and save it as python file ( .py )
- move to robot_tutorials folder >> create new folder called scripts 
- open the termenal and write " $ roscore " to start the master node
- open new window of terminal and navigate the directory of scripts folder
  write
  $ chmod +x Publish.py    // to chaneg the premissions of file
  $ python3 Publish.py
  
- repeate same steps on previous stage  with Subsecribe.py


