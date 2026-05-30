cmake_minimum_required(VERSION 3.8)
project(knowledge_bank)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY
    domains
    phrases
    runtime
    dictionaries
  DESTINATION share/${PROJECT_NAME}
)

ament_package()
