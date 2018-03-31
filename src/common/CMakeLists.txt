# Include path
include_directories(${CMAKE_CURRENT_SOURCE_DIR})

# Dependency libraries
# find_package(LIBRARY_NAME REQUIRED)

# Add libraries
add_library(common INTERFACE)
target_include_directories(common INTERFACE
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
  $<INSTALL_INTERFACE:include>)


