cmake_minimum_required(VERSION 3.0.2)
project(yolov5_msgs)

find_package(catkin REQUIRED COMPONENTS
  geometry_msgs
  std_msgs
  message_generation
)

add_message_files(
   FILES
   Object.msg
   Detection.msg
)

add_service_files(
   FILES
   PoseListArmCommand.srv
   NamedArmCommand.srv
)

generate_messages(
  DEPENDENCIES
  std_msgs
  geometry_msgs
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES yolov5_msgs
   CATKIN_DEPENDS message_runtime geometry_msgs std_msgs
#  DEPENDS system_lib
)

include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)
