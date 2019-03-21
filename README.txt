This is the package for ROS which based on the turtlebot follower package. 

To run this program, simply do:
roslaunch turtlebot_follower follower.launch

We modified the original cpp file to change the behavior of the robot. When the centroid is too far away, the robot goes very slowly towards the centroid until the distance is within the maximum distance in the range, then it will use the follower mode. If there is not enough points detected, the robot will slowly go forward while turning around, mimics the behavior of find an object to follow. 

For more details, please check http://wiki.ros.org/turtlebot_follower
