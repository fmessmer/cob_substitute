cmake_minimum_required(VERSION 3.0.2)
project(cob_docker_control)

find_package(catkin REQUIRED)

catkin_package()

install(PROGRAMS
  scripts/fake_docking.py
  scripts/multi_station_docker_control.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
