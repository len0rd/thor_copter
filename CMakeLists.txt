cmake_minimum_required(VERSION 2.8.3)
project(thorcopter)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  rosflight_msgs
  roscopter
  inertial_sense
  vrpn_client_ros
)

###################################
## catkin specific configuration ##
###################################
## The catkin_package macro generates cmake config files for your package
## Declare things to be passed to dependent projects
## INCLUDE_DIRS: uncomment this if you package contains header files
## LIBRARIES: libraries you create in this project that dependent projects also need
## CATKIN_DEPENDS: catkin_packages dependent projects also need
## DEPENDS: system dependencies of this project that dependent projects also need
catkin_package(
# INCLUDE_DIRS include
#  LIBRARIES thor
 CATKIN_DEPENDS roscopter rosflight_msgs inertial_sense vrpn_client_ros roscpp rospy
#  DEPENDS system_lib
)
add_definitions(-std=c++11)