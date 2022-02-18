cmake_minimum_required(VERSION 3.17)
project(Project1)

set(CMAKE_CXX_STANDARD 11)
set(GCC_COVERAGE_COMPILE_FLAGS "-lpthread -pthread")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${GCC_COVERAGE_COMPILE_FLAGS}")

add_executable(Project1 anomaly_detection_util.cpp anomaly_detection_util.h AnomalyDetector.h CLI.h CLI.cpp
        commands.h HybridAnomalyDetector.cpp HybridAnomalyDetector.h MainTrain.cpp minCircle.h minCircle.cpp
        SimpleAnomalyDetector.h SimpleAnomalyDetector.cpp timeseries.h timeseries.cpp Server.cpp Server.h)