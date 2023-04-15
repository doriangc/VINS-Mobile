
cmake_minimum_required(VERSION 3.4.1)
project(VINSMobile)

# SET(OpenCV_DIR {path}/OpenCV-android-sdk/sdk/native/jni)
find_package(OpenCV REQUIRED)
# add_definitions(-DOPENCV_DISABLE_EIGEN_TENSOR_SUPPORT)

# find_package(Ceres REQUIRED)
# find_package(Boost REQUIRED)
# find_package(Eigen3 REQUIRED)

# message("Ceres include dir: ${Ceres_INCLUDE_DIR}")
# message("Boost include dir: ${Boost_INCLUDE_DIR}")
# message("Eigen 3 include dir: ${Eigen3_INCLUDE_DIR}")

# message("Ceres libraries: ${Ceres_LIBRARIES}")
# message("Boost libraries: ${Boost_LIBRARIES}")
# message("Eigen 3 libraries: ${Eigen3_LIBRARIES}")


# include_directories(/usr/include/eigen3/)

# this is branching into all the subdirectories and thus connecting them all
add_subdirectory(VINS_ThirdPartyLib)
add_subdirectory(ThirdParty/DBoW)
add_subdirectory(ThirdParty/DUtils)
add_subdirectory(ThirdParty/DVision)
add_subdirectory(VINS_ios)
