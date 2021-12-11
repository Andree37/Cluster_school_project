cmake_minimum_required(VERSION 3.21)
project(Cluster_school_project C)

set(CMAKE_C_STANDARD 11)

file(COPY Projeto2Fase/Projeto2Fase/players.csv DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY Projeto2Fase/Projeto2Fase/games.csv DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

include_directories(Projeto2Fase/Projeto2Fase)

add_executable(Cluster_school_project
        Projeto2Fase/Projeto2Fase/cluster.c
        Projeto2Fase/Projeto2Fase/cluster.h
        Projeto2Fase/Projeto2Fase/commands.c
        Projeto2Fase/Projeto2Fase/commands.h
        Projeto2Fase/Projeto2Fase/date.c
        Projeto2Fase/Projeto2Fase/date.h
        Projeto2Fase/Projeto2Fase/list.h
        Projeto2Fase/Projeto2Fase/listArrayList.c
        Projeto2Fase/Projeto2Fase/listElem.c
        Projeto2Fase/Projeto2Fase/listElem.h
        Projeto2Fase/Projeto2Fase/main.c
        Projeto2Fase/Projeto2Fase/map.h
        Projeto2Fase/Projeto2Fase/mapArrayList.c
        Projeto2Fase/Projeto2Fase/mapElem.c
        Projeto2Fase/Projeto2Fase/mapElem.h
        Projeto2Fase/Projeto2Fase/player.c
        Projeto2Fase/Projeto2Fase/player.h
        Projeto2Fase/Projeto2Fase/playerType.c
        Projeto2Fase/Projeto2Fase/playerType.h
        Projeto2Fase/Projeto2Fase/statistics.c
        Projeto2Fase/Projeto2Fase/statistics.h)
