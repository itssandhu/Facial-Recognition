cmake_minimum_required(VERSION 3.12)
project(FacialRecognition)

# Set C++ standard
set(CMAKE_CXX_STANDARD 11)

# Find OpenCV
find_package(OpenCV REQUIRED)

# Add your source files
add_executable(face main.cpp)

# Link OpenCV
target_link_libraries(face PRIVATE ${OpenCV_LIBS})
