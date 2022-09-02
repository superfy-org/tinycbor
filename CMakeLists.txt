if(CONFIG_TINYCBOR_SUPERFY)
  zephyr_include_directories(
    ${ZEPHYR_TINYCBOR_SUPERFY_MODULE_DIR}/src
  )

  zephyr_library()
  zephyr_library_sources(
    ${ZEPHYR_TINYCBOR_SUPERFY_MODULE_DIR}/src/cborencoder_close_container_checked.c
    ${ZEPHYR_TINYCBOR_SUPERFY_MODULE_DIR}/src/cborencoder.c
    ${ZEPHYR_TINYCBOR_SUPERFY_MODULE_DIR}/src/cborerrorstrings.c
    ${ZEPHYR_TINYCBOR_SUPERFY_MODULE_DIR}/src/cborparser_dup_string.c
    ${ZEPHYR_TINYCBOR_SUPERFY_MODULE_DIR}/src/cborparser.c
    ${ZEPHYR_TINYCBOR_SUPERFY_MODULE_DIR}/src/cborvalidation.c
    ${ZEPHYR_TINYCBOR_SUPERFY_MODULE_DIR}/src/cborpretty.c
    ${ZEPHYR_TINYCBOR_SUPERFY_MODULE_DIR}/src/cborpretty_stdio.c
  )
endif()
