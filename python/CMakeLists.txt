pybind11_add_module(maestro _maestro.cc _maestro_CA.cc _maestro_API.cc _maestro_DFA.cc)
target_link_libraries(maestro PRIVATE maestro-core)

# turn all the warnings on
target_compile_options(maestro PRIVATE -Wall -Wextra)
