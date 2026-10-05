
add_executable(
    lesson_002
    main.cpp
)

target_compile_options(
    lesson_002
    PRIVATE
        -Wall
        -Wextra
        -Wpedantic
)