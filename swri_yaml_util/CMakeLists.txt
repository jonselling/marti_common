cmake_minimum_required(VERSION 3.16)
project(swri_yaml_util)

find_package(catkin REQUIRED COMPONENTS
  roscpp
)

find_package(PkgConfig)
pkg_check_modules(YamlCpp yaml-cpp)
message(STATUS "YAML-CPP VERSION: " ${YamlCpp_VERSION})
message(STATUS "YAML-CPP LIBRARY: " ${YamlCpp_LIBRARIES})

catkin_destinations()
file(MAKE_DIRECTORY ${CATKIN_DEVEL_PREFIX}/${CATKIN_PACKAGE_INCLUDE_DESTINATION})
catkin_package(
  INCLUDE_DIRS include ${CATKIN_DEVEL_PREFIX}/${CATKIN_GLOBAL_INCLUDE_DESTINATION}
  LIBRARIES ${PROJECT_NAME} ${YamlCpp_LIBRARIES}
  CATKIN_DEPENDS roscpp
)

if( ${YamlCpp_VERSION} MATCHES "0.[23].*")
  set(YAMLCPP_OLD_API ON)
  message(STATUS "  Using old yaml-cpp API.")
else()
  set(YAMLCPP_OLD_API OFF)
  message(STATUS "  Using new yaml-cpp API.")
endif()

configure_file(version.h.in ${CATKIN_DEVEL_PREFIX}/${CATKIN_PACKAGE_INCLUDE_DESTINATION}/version.h)

include_directories(include)
include_directories(SYSTEM
  ${catkin_INCLUDE_DIRS}
  ${CATKIN_DEVEL_PREFIX}/${CATKIN_GLOBAL_INCLUDE_DESTINATION}
  ${YamlCpp_INCLUDE_DIRS}
)

add_library(${PROJECT_NAME}
  src/yaml_util.cpp
)

target_compile_features(${PROJECT_NAME} PUBLIC cxx_std_14)

target_link_libraries(${PROJECT_NAME}
  ${catkin_LIBRARIES}
  ${YamlCpp_LIBRARIES}
)

install(DIRECTORY include/${PROJECT_NAME}/
  DESTINATION ${CATKIN_PACKAGE_INCLUDE_DESTINATION}
  FILES_MATCHING PATTERN "*.h"
)

install(
  DIRECTORY ${CATKIN_DEVEL_PREFIX}/${CATKIN_PACKAGE_INCLUDE_DESTINATION}/
  DESTINATION ${CATKIN_PACKAGE_INCLUDE_DESTINATION}
)

install(TARGETS ${PROJECT_NAME}
  RUNTIME DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
  LIBRARY DESTINATION ${CATKIN_PACKAGE_LIB_DESTINATION}
  ARCHIVE DESTINATION ${CATKIN_PACKAGE_LIB_DESTINATION}
)

