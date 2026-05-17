
idf_component_register(SRCS "main.c"
                    INCLUDE_DIRS ".")

# Speed test: disable USB stack logs in data path (overrides default USB_DBG_INFO)
target_compile_definitions(${COMPONENT_LIB} PRIVATE CONFIG_USB_DBG_LEVEL=0)
