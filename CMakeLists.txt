cmake_minimum_required(VERSION 3.4.1)
project("android-opencv-opengl-assignment")

# Add native-lib
add_library(native-lib SHARED jni/native-lib.cpp)

find_library(log-lib log)

# Example OpenCV linking (adjust OpenCV_DIR path on your machine)
# set(OpenCV_DIR /path/to/OpenCV-android-sdk/sdk/native/jni)
# find_package(OpenCV REQUIRED)
# include_directories(${OpenCV_INCLUDE_DIRS})
# target_link_libraries(native-lib ${OpenCV_LIBS} ${log-lib})

# If not using OpenCV yet, link log only
target_link_libraries(native-lib ${log-lib})
