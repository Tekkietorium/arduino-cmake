set(CMAKE_TOOLCHAIN_FILE %{TOOLCHAIN})

cmake_minimum_required(VERSION 2.8.12)
project(%{ProjectName})

set(ARDUINO_EXTRA_LIBRARIES_PATH 
  $ENV{HOME}/Arduino/libraries
  ${ARDUINO_SDK_PATH}/hardware/arduino/avr/libraries
)

set(ARDUINO_DEFAULT_BOARD %{BOARD}) # Default Board ID, when not specified
set(ARDUINO_DEFAULT_PORT %{PORT}) # Default Port, when not specified

generate_arduino_firmware(${PROJECT_NAME} SRCS %{ProjectName}.ino)
