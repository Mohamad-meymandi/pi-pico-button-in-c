cmake_minimum_required(VERSION 3.13)


# initialize the SDK based on PICO_SDK_PATH
# note: this must happen before project()
include(pico_sdk_import.cmake)


# initialize the Raspberry Pi Pico SDK
pico_sdk_init()

# rest of your project

add_executable(Button

	main.c
)

target_link_libraries(Button pico_stdlib)

pico_add_extra_outputs(Button)

#example_auto_set_url(blink)

