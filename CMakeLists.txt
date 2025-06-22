idf_component_register(SRCS "mongoose.c" INCLUDE_DIRS ".")

target_compile_definitions(${COMPONENT_LIB}
  PUBLIC
    MG_ARCH=MG_ARCH_UNIX
    MG_ENABLE_POLL=1
    MG_IO_SIZE=2048
)
