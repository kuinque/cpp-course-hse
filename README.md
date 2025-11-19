# HSE C++ Course Archive

This repository contains two comprehensive C++ course repositories from HSE (Higher School of Economics) University:

1. [**cpp-advanced-hse**](https://github.com/kuinque/hse-Ilia-Krivetskii-quinque) - Advanced C++ course covering modern C++ features, concurrency, memory management, and advanced topics
2. [**hse-cpp-problems**](https://github.com/kuinque/hse-cpp-problems) - Introductory C++ course with fundamental programming problems and algorithms

## Repository Overview

### 📚 cpp-advanced-hse

**Advanced C++ Course** - A comprehensive course covering advanced C++ programming concepts, modern C++ standards (C++17/C++20), and system programming topics.

#### Key Features:
- **Modern C++ Standards**: Uses C++17 and C++20 features extensively
- **Compiler**: Built with clang-18 (minimum clang-11 for C++20 support)
- **Testing Framework**: Catch2, Google Test (GTest), Google Mock (GMock)
- **Build System**: CMake 3.13+
- **Code Style**: Google C++ Style Guide with modifications
- **Platform**: Primarily Linux (Ubuntu 24.04 recommended), macOS supported, Windows via WSL2

#### Course Structure:

**Weekly Homeworks:**
- **intro/** - Introduction tasks (GCD, multiplication)
- **memory/** - Memory management (dedup, deque, intrusive-list, LRU cache, string-view)
- **move/** - Move semantics (compressed-pair, COW vector, harakiri, string operations)
- **types/** - Type system (dungeon, fold, functors, itertools)
- **errors/** - Error handling (defer, grep, safe-transform, tryhard)
- **patterns/** - Design patterns (any, editor, pimpl, scala-vector, small-test-framework)
- **meta/** - Metaprogramming (compile-eval, constexpr-map, function-ref)
- **baby-threads/** - Basic multithreading (hash-table, is-prime, reduce, subset-sum)
- **condvars/** - Condition variables and synchronization (buffered-channel, rw-lock, semaphore, timerqueue, unbuffered-channel)
- **lock-free/** - Lock-free programming (fast-queue, futex, hazard-ptr, mpsc-stack, rw-spinlock, sync-map)

**Major Projects:**
- **smart-ptrs/** - Smart pointer implementation (UniquePtr, SharedPtr, WeakPtr, IntrusivePtr, SharedFromThis) - 10 points total
- **scheme/** - Scheme/LISP interpreter implementation (tokenizer, parser, basic, advanced, tidy with garbage collection) - 10 points total
- **jpeg-decoder/** - JPEG decoder implementation (baseline, progressive, faster, huffman, FFTW variants)

**Bonus Tasks:**
- **bonus/** - Advanced challenges (bad-hash, bad-rand, clang-fun, executors, functional-world, hack-cpp, matrix-2.0, solve-or-die)

**Additional Resources:**
- **seminars/** - Seminar materials and examples (2021-2024)
- **lectures/** - Lecture materials (2021-2023)
- **docs/** - Documentation (setup, troubleshooting, multithreading, questions, etc.)
- **allocations_checker/** - Custom allocation checker tool
- **contrib/** - Third-party dependencies (benchmark, catch, gmock, gtest)

#### Testing and Submission:
- Automated testing via GitLab CI/CD
- Submission via `submit.py` script
- Web interface for deadlines and grades: https://cpp-hse.net
- Private student repositories on GitLab

#### Documentation:
- Setup guide: `docs/setup.md`
- Troubleshooting: `docs/troubleshooting.md`
- Multithreading guide: `docs/multithreading.md`
- Questions guide: `docs/questions.md`
- Windows setup: `docs/windows.md`

---

### 📖 hse-cpp-problems

**Introductory C++ Course** - A foundational C++ programming course covering basic to intermediate programming concepts and algorithms.

#### Key Features:
- **C++ Standard**: C++11/C++17
- **Compiler**: clang-11
- **Testing Framework**: Catch2
- **Build System**: CMake 3.8+
- **Code Style**: Google C++ Style Guide (strict adherence required)
- **Platform**: Linux (Ubuntu 20.04 recommended)

#### Course Structure:

**Level 0:**
- **multiplication/** - Introduction task (familiarization with testing system)

**Level 1: Basic Algorithms:**
- **next_even/** - Next even number
- **is_leap/** - Leap year detection
- **chocolate/** - Chocolate bar problem
- **min_divisor/** - Minimum divisor
- **fibonacci/** - Fibonacci sequence
- **reduce_fraction/** - Fraction reduction
- **palindrome/** - Palindrome detection
- **password/** - Password validation

**Level 2: Data Structures and Algorithms:**
- **sort_students/** - Student sorting
- **tests_checking/** - Test validation
- **admission/** - Admission system
- **scorer/** - Scoring system
- **unixpath/** - Unix path manipulation

**Level 3: Advanced Topics:**
- **provinces/** - Graph/connectivity problems
- **search/** - Search algorithms
- **rational/** - Rational number class
- **stack/** - Stack data structure
- **queue/** - Queue data structure

**Project:**
- **image_processor/** - Image processing application (BMP format, filters: blur, crop, edge, greyscale, negative, retro, sharp)

#### Testing and Submission:
- Automated testing via GitLab CI/CD
- Submission via Git branches (`submits/task_name`)
- Web interface: https://base.cpp-hse.net
- Private student repositories on GitLab

#### Documentation:
- Setup guide: `SETUP.md`
- Style guide: `STYLEGUIDE.md` (comprehensive C++ coding standards)
- Score tracking: `SCORE.md`
- Lectures: `LECTURES.md`

---

## Common Features

### Build System
Both repositories use CMake for building:
```bash
mkdir build
cd build
cmake ..
make <target_name>
```

### Code Style
- Google C++ Style Guide with modifications
- 2-4 space indentation (consistent within project)
- Maximum line length: 100-120 characters
- clang-format for automatic formatting
- Strict linting requirements

### Testing
- Unit tests using Catch2 framework
- Hidden test cases on submission
- Automated CI/CD pipeline
- Local testing before submission

### Development Environment
- **Recommended**: Ubuntu (24.04 for advanced, 20.04 for intro)
- **Alternative**: macOS, Windows with WSL2
- **IDEs**: CLion, VSCode, Vim, Sublime
- **Language Server**: clangd recommended for IDE support

### Git Workflow
- Main repository for tasks and updates
- Private student repositories for submissions
- Regular updates via `git pull`
- Branch-based submission (hse-cpp-problems) or direct submission (cpp-advanced-hse)

---

## Getting Started

### For cpp-advanced-hse:
1. Clone the repository: `git clone https://gitlab.com/hse-cpp/cpp-advanced-hse`
2. Follow setup instructions in `docs/setup.md`
3. Register at https://cpp-hse.net
4. Configure your private repository
5. Start with tasks in `tasks/intro/`

### For hse-cpp-problems:
1. Clone your private repository from GitLab
2. Follow setup instructions in `SETUP.md`
3. Register at https://base.cpp-hse.net
4. Start with `tasks/multiplication/` (intro task)
5. Work through tasks in order

---

## Project Statistics

### cpp-advanced-hse:
- **Total Tasks**: 50+ tasks across 10+ categories
- **Major Projects**: 3 (Smart Pointers, Scheme Interpreter, JPEG Decoder)
- **Bonus Tasks**: 8 advanced challenges
- **Seminars**: Materials from 2021-2024
- **Lectures**: Materials from 2021-2023

### hse-cpp-problems:
- **Total Tasks**: 20+ tasks across 4 difficulty levels
- **Project**: 1 major project (Image Processor)
- **Focus**: Algorithms, data structures, and C++ fundamentals

---

## Key Learning Outcomes

### cpp-advanced-hse:
- Modern C++ features (C++17/C++20)
- Memory management and smart pointers
- Move semantics and perfect forwarding
- Template metaprogramming
- Concurrency and multithreading
- Lock-free programming
- Design patterns
- System programming

### hse-cpp-problems:
- C++ fundamentals
- Algorithm implementation
- Data structures
- Object-oriented programming
- Code organization and style
- Testing and debugging

---

## Notes

- Both courses emphasize code quality, testing, and proper C++ style
- Solutions must pass automated tests and code review
- Regular updates to task repositories require synchronization
- Academic integrity is strictly enforced
- All code follows Google C++ Style Guide with project-specific modifications


