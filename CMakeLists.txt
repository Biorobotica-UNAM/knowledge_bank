cmake_minimum_required(VERSION 3.8)
project(knowledge_bank)

find_package(ament_cmake REQUIRED)

# Instalar las carpetas reales que contienen tus archivos YAML
install(
  DIRECTORY
    keys
    phrases
    save
    say
    volatile
  DESTINATION share/${PROJECT_NAME}
)

ament_package()