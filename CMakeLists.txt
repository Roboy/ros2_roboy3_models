cmake_minimum_required(VERSION 3.8)
project(ros2_roboy3_models)

# Default to C++14
if(NOT CMAKE_CXX_STANDARD)
  set(CMAKE_CXX_STANDARD 14)
endif()

find_package(ament_cmake REQUIRED)


install(FILES
        package.xml
        DESTINATION share/${PROJECT_NAME}
        )

ament_package()
