cmake_minimum_required(VERSION 3.0.2)
project(yolov5_ros)

find_package(catkin REQUIRED
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES yolov5_ros
#  CATKIN_DEPENDS message_runtime
#  DEPENDS system_lib
)

include_directories(
# include
# ${catkin_INCLUDE_DIRS}
)
