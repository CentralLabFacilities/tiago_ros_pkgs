cmake_minimum_required(VERSION 2.8.3)
project(tiago_clf_launch)

find_package(catkin REQUIRED)

catkin_package()

install(PROGRAMS
    scripts/clf_joy
    scripts/joy_teleop
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)

install(DIRECTORY launch DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
install(DIRECTORY config DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
