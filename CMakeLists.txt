idf_component_register(SRCS "mongoose.c" INCLUDE_DIRS "." REQUIRES mbedtls)

target_compile_definitions(${COMPONENT_LIB}
  PUBLIC
    MG_ARCH=MG_ARCH_UNIX
    MG_ENABLE_CUSTOM_RANDOM=1
    MG_ENABLE_POLL=0
    MG_IO_SIZE=2048
    MG_TLS=MG_TLS_MBED
)
