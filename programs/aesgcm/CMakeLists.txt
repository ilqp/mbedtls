add_executable(aesgcm aesgcm.c)
target_link_libraries(aesgcm mbedaesgcm)

install(TARGETS aesgcm
        DESTINATION "bin"
        PERMISSIONS OWNER_READ OWNER_WRITE OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE)
