cmake_minimum_required(VERSION 3.16.3)
project(GAME_PROJ)

set(CMAKE_CXX_STANDARD 17)

add_executable(GAME_PROJ sources/main.cpp sources/cell.cpp sources/cellObject.cpp sources/field_view.cpp sources/field.cpp sources/game.cpp sources/player.cpp sources/enemyBoss.cpp sources/enemyMove.cpp sources/enemyStand.cpp sources/objectHeal.cpp sources/objectDamage.cpp sources/objectRange.cpp sources/cellView.cpp sources/cellObjectView.cpp
headers/cell.h headers/cellObject.h headers/field_view.h headers/field.h headers/game.h headers/player.h headers/enemyInterface.h headers/enemyBoss.h headers/enemyMove.h headers/enemyStand.h headers/objectHeal.h headers/objectDamage.h headers/objectRange.h headers/cellView.h headers/cellObjectView.h)

target_link_libraries(GAME_PROJ sfml-graphics sfml-window sfml-system -lncurses -g)