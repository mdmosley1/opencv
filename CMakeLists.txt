cmake_minimum_required(VERSION 2.8)
project( DisplayImage )
find_package( OpenCV REQUIRED )

add_executable( DisplayImage DisplayImage.cpp )
add_executable( DisplayVideo DisplayVideo.cpp )
add_executable( Trackbar Trackbar.cpp )

target_link_libraries( DisplayImage ${OpenCV_LIBS} )
target_link_libraries( DisplayVideo ${OpenCV_LIBS} )
target_link_libraries( Trackbar ${OpenCV_LIBS} )
