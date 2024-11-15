# GrayScott Reaction-Diffusion Simulation System

This project is a GrayScott project template based on the GoogleTest framework, designed to demonstrate unit testing, build system configuration, and CI/CD pipeline for C++ projects. The project uses CMake for building and supports automated building and testing in both `Debug` and `Release` modes.

## 🚀 Key Features

- Implementation of the Gray-Scott reaction-diffusion model
- Complete testing framework based on GoogleTest
- Support for both Debug and Release build modes
- Continuous integration using GitHub Actions
- Cross-platform support (Linux, macOS, and Windows)

## 📋 Requirements

Building and running this project requires:
- C++ compiler with C++14 support
- CMake (version 3.14 or higher)
- GoogleTest framework
- Git

## 📦 Project Structure

```
GrayScott/
├── build/              # Generated libraries and executables
├── ci/                 # Continuous integration scripts
│   ├── linux-presubmit.sh
│   ├── macos-presubmit.sh
│   └── windows-presubmit.bat
├── docs/               # Project documentation
│   ├── primer.md
│   ├── quickstart-cmake.md
│   ├── advanced.md
│   └── faq.md
├── include/            # Header files directory
├── src/               # Source files directory
│   └── gs.cpp        # Main implementation
├── tests/            # Test files directory
│   └── gs_test.cpp  # Unit tests
├── CMakeLists.txt    # CMake build configuration
└── .github/workflows/ # CI configuration
    └── ci.yml        # GitHub Actions workflow
```

## 🛠️ Building the Project

### Build Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/GrayScott.git
   cd GrayScott
   ```

2. **Create build directory**:
   ```bash
   mkdir build
   cd build
   ```

3. **Choose build mode and build the project**:
   
   Debug mode:
   ```bash
   cmake -DCMAKE_BUILD_TYPE=Debug ..
   make
   ```
   
   Release mode:
   ```bash
   cmake -DCMAKE_BUILD_TYPE=Release ..
   make
   ```

### Running Applications and Tests

1. **Run the main program**:
   ```bash
   ./build/gs_main
   ```

2. **Run unit tests**:
   ```bash
   ./build/gs_test
   ```

## 👥 Team Roles and Responsibilities

### Repository Setup and Git Management (Member A)
- Maintain code version control and Git conventions
- Manage branching model:
  - Main branch (`main`): stable releases
  - Development branch (`dev`): latest code integration
  - Feature branches (`feature/xxx`): independent development
- Establish code submission guidelines and review process

### Testing Framework and Unit Tests (Member B)
- Configure GoogleTest framework
- Write unit tests of varying complexity
- Ensure test coverage of core functionality
- Maintain test documentation

### Build System Implementation (Member C)
- Configure and maintain CMake build system
- Ensure correctness of Debug and Release build modes
- Implement automatic compilation and linking
- Verify build process

### Continuous Integration Setup (Member D)
- Configure GitHub Actions workflow
- Implement automated testing process
- Manage multi-platform testing (Linux, macOS, Windows)
- Set up build failure notification system

### Documentation Writing and Maintenance (Member E)
- Write project documentation and user guides
- Maintain technical documentation
- Create presentation materials
- Document team contributions

## 🔄 Continuous Integration

The project uses GitHub Actions for continuous integration, including:
- Automated building and testing
- Multi-platform compatibility testing
- Debug and Release mode verification
- Failure notification mechanism

Local testing scripts:
```bash
./ci/linux-presubmit.sh   # Linux
./ci/macos-presubmit.sh   # macOS
./ci/windows-presubmit.bat # Windows
```

## 📚 Documentation

Detailed documentation is located in the `docs/` directory:
- `primer.md`: Project basics guide
- `quickstart-cmake.md`: CMake quick start
- `advanced.md`: Advanced features guide
- `faq.md`: Frequently asked questions

## ⚖️ License

[Add your chosen license here]

## 📬 Contact

[Add your contact information here]

## Acknowledgments

This project is based on GoogleTest and GoogleMock. For more information, see the [GoogleTest official documentation](https://github.com/google/googletest).

---
*Note: This project is under active development. Please report any issues or suggestions through the GitHub issue tracker.*
