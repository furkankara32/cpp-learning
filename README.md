# Modern C++ Learning

A structured Modern C++ learning repository focused on building a strong
C++11/14/17 foundation for **Embedded Software Development**.

This repository contains my notes, examples, exercises, and small projects
while studying the **Complete Modern C++ (C++11/14/17)** course by
**Umar Lone**.

My main goal is not only to learn the C++ language, but also to understand
how Modern C++ concepts can be applied to embedded systems, firmware
architecture, and ROS2 development.

---

## Learning Goals

The main topics covered in this repository include:

- C++ compilation process
- References and pointers
- `const` correctness
- Function overloading
- Classes and objects
- Constructors and destructors
- Copy semantics
- Move semantics
- Rule of 5 and Rule of 0
- Operator overloading
- Dynamic memory management
- RAII and resource management
- Smart pointers
- Inheritance and polymorphism
- Templates
- Lambda expressions
- Standard Template Library (STL)
- Exception handling
- File I/O
- C++ concurrency
- C++17 language features
- C++17 standard library features

## Development Environment

The course examples are developed on Linux using the following toolchain:

| Tool | Purpose |
|---|---|
| Ubuntu | Development operating system |
| VS Code | Source code editor |
| GCC / G++ | C/C++ compiler toolchain |
| CMake | Build system configuration |
| GDB | Debugger |
| Git | Version control |
| GitHub | Remote repository |

The project currently targets:

```text
C++17
```

---

## Repository Structure

```text
cpp-learning/
│
├── lessons/
│   ├── 001_hello_world/
│   │   ├── CMakeLists.txt
│   │   └── main.cpp
│   │
│   ├── 002_...
│   └── ...
│
├── exercises/
│   └── ...
│
├── projects/
│   └── ...
│
├── CMakeLists.txt
├── .gitignore
└── README.md
```

### `lessons/`

Contains examples written while progressing through the course.

Each topic is kept separately so previous examples remain available for
future reference.

### `exercises/`

Contains additional exercises written to reinforce C++ concepts.

Where possible, exercises will be adapted to embedded software scenarios
such as:

```text
UART
SPI
GPIO
Sensors
Ring Buffers
State Machines
RTOS Resources
```

### `projects/`

Contains larger applications combining multiple Modern C++ concepts.

Future projects may include:

- C++ GPIO abstraction
- UART driver abstraction
- SPI device interface
- Sensor driver architecture
- RAII-based resource guards
- Embedded-friendly ring buffer
- FreeRTOS C++ wrappers
- ROS2 sensor node

---

## Building the Project

Configure the project:

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Debug
```

Build:

```bash
cmake --build build
```

For example, run the first lesson:

```bash
./build/lessons/001_hello_world/lesson_001
```

---

## Debugging

Executables can be debugged using GDB:

```bash
gdb ./build/lessons/001_hello_world/lesson_001
```

Common GDB commands:

```text
break main
run
next
step
continue
print <variable>
quit
```

VS Code and CMake Tools are also configured for graphical debugging with
breakpoints, variable inspection, call stacks, and step-by-step execution.

---

## Learning Path

The repository will roughly follow this progression:

```text
C++ Fundamentals
       │
       ▼
Pointers & References
       │
       ▼
Classes & Objects
       │
       ▼
Constructors / Destructors
       │
       ▼
Memory Management
       │
       ▼
Copy & Move Semantics
       │
       ▼
RAII
       │
       ▼
OOP
       │
       ▼
Templates
       │
       ▼
Lambda Expressions
       │
       ▼
STL
       │
       ▼
Concurrency
       │
       ▼
Modern C++17
       │
       ▼
Embedded C++
       │
       ├── STM32
       ├── FreeRTOS
       └── Sensor Drivers
       │
       ▼
ROS2 C++
```

---
## Course

**Complete Modern C++ (C++11/14/17)**  
Instructor: **Umar Lone**

The course is used as the main learning resource, while this repository
extends the material with additional exercises and embedded-oriented
examples.

---

## License

This repository contains my own learning notes, source code, exercises, and
implementations.

Course materials and original course content belong to their respective
author and publisher.