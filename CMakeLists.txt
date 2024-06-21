cmake_minimum_required(VERSION 3.5)
project(my_robot_description)

# Find dependencies
find_package(ament_cmake REQUIRED)

# Install launch files
install(
  DIRECTORY launch rviz urdf
  DESTINATION share/${PROJECT_NAME}/
)

ament_package()
