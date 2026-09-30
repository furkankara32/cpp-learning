
add_executable(
    lesson_001
    main.cpp
)

target_compile_options(
    lesson_001
    PRIVATE
        -Wall
        -Wextra
        -Wpedantic
)