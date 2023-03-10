cmake_minimum_required(VERSION 3.1...3.14)

project(chapter_20 LANGUAGES CXX)

catch_add_test(buffers buffers.cpp)
add_executable(asio asio.cpp)
add_executable(name_resolution name_resolution.cpp)
add_executable(name_resolution_async name_resolution_async.cpp)
add_executable(connect connect.cpp)
add_executable(connect_async connect_async.cpp)
add_executable(web_request web_request.cpp)
add_executable(web_request_async web_request_async.cpp)
add_executable(web_request_async_multi web_request_async_multi.cpp)
add_executable(upper_echo_server upper_echo_server.cpp)
add_executable(upper_echo_server_async upper_echo_server_async.cpp)
add_executable(upper_echo_server_multi upper_echo_server_multi.cpp)

target_link_libraries(asio PRIVATE CONAN_PKG::boost)
target_link_libraries(name_resolution PRIVATE CONAN_PKG::boost)
target_link_libraries(name_resolution_async PRIVATE CONAN_PKG::boost)
target_link_libraries(connect PRIVATE CONAN_PKG::boost)
target_link_libraries(connect_async PRIVATE CONAN_PKG::boost)
target_link_libraries(web_request PRIVATE CONAN_PKG::boost)
target_link_libraries(web_request_async PRIVATE CONAN_PKG::boost)
target_link_libraries(web_request_async_multi PRIVATE CONAN_PKG::boost)
target_link_libraries(buffers PRIVATE CONAN_PKG::boost)
target_link_libraries(upper_echo_server PRIVATE CONAN_PKG::boost)
target_link_libraries(upper_echo_server_async PRIVATE CONAN_PKG::boost)
target_link_libraries(upper_echo_server_multi PRIVATE CONAN_PKG::boost)
