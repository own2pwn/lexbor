cmake_minimum_required(VERSION 2.8)

################
## Search and Includes
#########################
include_directories(".")

################
## Sources
#########################
file(GLOB_RECURSE FUZZ_LEXBOR_HTML_SOURCES "*.c")

################
## Create
#########################
EXECUTABLE_LIST("fuzz_lexbor_html_" "${FUZZ_LEXBOR_HTML_SOURCES}" ${TEST_UNIT_LIB_NAME} ${LEXBOR_LIB_NAME})
