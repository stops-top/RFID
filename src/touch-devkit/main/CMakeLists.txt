if(IDF_TARGET STREQUAL "esp32s2")
    idf_component_register(SRCS "main.c"
                            INCLUDE_DIRS ".")
else()
    message(FATAL_ERROR "Touch app create example only available on esp32s2 now")
endif()
