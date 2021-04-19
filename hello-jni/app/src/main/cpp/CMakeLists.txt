cmake_minimum_required(VERSION 3.4.1)


# 定义一个库
add_library(hello-jni SHARED
            hello-jni.c)

# Include libraries needed for hello-jni lib

# 添加库用到的api库
target_link_libraries(hello-jni
                      android
                      log)
