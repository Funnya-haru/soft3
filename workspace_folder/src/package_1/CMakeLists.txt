find_package(catkin REQUIRED COMPONENTS
  message_generation
  message_runtime
  roscpp
  rospy
  std_msgs
  geometry_msgs
  actionlib actionlib_msgs
)

add_action_files(FILES DoDishes.action)

generate_messages(DEPENDENCIES geometry_msgs actionlib_msgs)