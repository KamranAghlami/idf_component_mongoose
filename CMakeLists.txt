idf_component_register(SRCS "mongoose.c" INCLUDE_DIRS "." PRIV_REQUIRES lwip mbedtls)

target_compile_definitions(${COMPONENT_LIB} PRIVATE MG_ENABLE_MBEDTLS=1)
