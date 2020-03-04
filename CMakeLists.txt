cmake_minimum_required(VERSION 3.0.2)
project(message_generation)

find_package(catkin REQUIRED)

set(DEFAULT_MESSAGE_GENERATION_PACKAGES gencpp;geneus;gennodejs;genlisp;genmsg;genpy)
set(MESSAGE_GENERATION_PACKAGES "${DEFAULT_MESSAGE_GENERATION_PACKAGES}" CACHE STRING "")

catkin_package(CATKIN_DEPENDS ${MESSAGE_GENERATION_PACKAGES})
