cmake_minimum_required(VERSION 2.8.3)
project(drift_correction)

set(CMAKE_CXX_FLAGS "-std=c++0x ${CMAKE_CXX_FLAGS}")

set(ROS_CXX_DEPENDENCIES
  geometry_msgs
  ar_pose_msgs
  std_msgs
  std_srvs
  tf
  roscpp
)

find_package(catkin REQUIRED COMPONENTS
  ${ROS_CXX_DEPENDENCIES}
)

catkin_package(
   CATKIN_DEPENDS ${ROS_CXX_DEPENDENCIES}
)

