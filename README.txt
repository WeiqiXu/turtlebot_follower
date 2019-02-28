This is the package for ROS which based on the turtlebot follower package. We changed the c++ file name to LongFollower.cpp. In the cpp file, we change the namespace to turtlebot_follower and the class to LongFollower.

We modified the launch file (follower_1.launch) and the plugin file (nodules.xml) according to our package name and class name. 

For problem 1-3, we mainly modified the launch file, changed the according parameters to adjust the robot's behaviors.

For problem 4, we also modified the cpp file to change the behavior of the robot. When the centroid is too far away, the robot goes very slowly towards the centroid until the distance is within the maximum distance in the range, then it will use the follower mode. If there is not enough points detected, the robot will slowly go forward while turning around, mimics the behavior of find an object to follow. 
