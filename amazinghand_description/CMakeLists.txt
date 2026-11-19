cmake_minimum_required(VERSION 3.14)
project(amazinghand_description)

find_package(ament_cmake REQUIRED)

install(DIRECTORY config urdf meshes
  DESTINATION share/${PROJECT_NAME}
)

install(DIRECTORY rviz
  DESTINATION share/${PROJECT_NAME}
  OPTIONAL
)

ament_package()
