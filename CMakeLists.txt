add_library(mbed-blackpill-f401ce INTERFACE)

target_sources(mbed-blackpill-f401ce
    INTERFACE
        PeripheralPins.c
        system_clock.c
)

target_include_directories(mbed-blackpill-f401ce
    INTERFACE
        .
)

target_link_libraries(mbed-blackpill-f401ce INTERFACE mbed-stm32f401xe)
