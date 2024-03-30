cmake_minimum_required(VERSION 3.5)
project(ros2_roboy3_models)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY config meshes urdf
  DESTINATION share/${PROJECT_NAME}
)

ament_environment_hooks("${CMAKE_CURRENT_SOURCE_DIR}/env-hooks/${PROJECT_NAME}.dsv.in")

ament_package()
