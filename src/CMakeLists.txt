add_executable(PepeFrog server/main.cpp)

TARGET_LINK_LIBRARIES(PepeFrog LINK_PUBLIC ${Boost_LIBRARIES} )
target_link_libraries(PepeFrog dpp)

target_include_directories(PepeFrog PRIVATE libs/DPP/include)

set_target_properties(PepeFrog PROPERTIES CXX_STANDARD 17 CXX_STANDARD_REQUIRED ON)