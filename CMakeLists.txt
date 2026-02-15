cmake_minimum_required(VERSION 3.8)
project(knowledge_bank)

find_package(ament_cmake REQUIRED)

# Instalar todas las carpetas de acciones
install(
  DIRECTORY
    align
    approach
    check
    drop
    find
    fold
    follow
    goto
    listen
    point
    save
    say
    take
    wait
  DESTINATION share/${PROJECT_NAME}
)

ament_package()

