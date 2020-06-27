# ORBSLAM2_drone_mono

Clone this repository on your carkin_ws/src folder

run 'catkin_make'

run 'source devel/setup.bash 

To run the simulation:

'roslaunch move_robot all_nodes_parrot_move.launch'

This will launch the gazebo environment with sjtu drone with a monocular front camera

open rviz running on console 'rviz rviz'

and set the camera/image_raw topic for visualization of the orb features

and other topics you wish to see

To start the orbslam routine publish a empty message on the takeoff topic

run 'rostopic pub /drone/takeoff std_msgs/Empty "{}"'

to control the drone run 'rosrun teleop_twist_keyboard teleop_twist_keyboard.py'

to save the collected data use the rosbag package: 'http://wiki.ros.org/rosbag'

and to do comparisons on the data use the evo package from Michael Grupp: 'https://github.com/MichaelGrupp/evo/wiki/evo_traj'
