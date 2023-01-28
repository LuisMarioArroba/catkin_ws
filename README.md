In order to achive control of the robot, sincronize with gazebo, your must instal:
pip3 install pyyaml
pip3 install rospkg

To initiate the gazebo:
roslaunch kr150_gazebo kr150_gazebo.launch gripper_2f:=true camera_arm:=true

To control the movement of the band:
roslaunch kuka_2f_cam_moveit moveit_rviz.launch 

To activate control sistem of the robot:
roslaunch kuka_2f_cam_moveit move_group.launch
roslaunch kuka_2f_cam_moveit moveit_rviz.launch 

To control the gripper:
stopic pub /gripperripper_cmd/goal [Tap] [Tap]
(It is suggest to use the position of 0.42 for this type of boxes)
