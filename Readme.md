# Basic C++ CMake Project

A modern CMake-based C++ project template for Linux environments.

## Project Structure

- `src/` - Source files
- `include/` - Header files
- `external/` - Third-party dependencies
- `tests/` - Project tests using Catch2
- `build/` - Build directory (generated)

## Requirements

- CMake 3.10 or higher
- C++17 compliant compiler (GCC or Clang)
- Git

## Building the Project

```bash
# Create and enter build directory
mkdir -p build && cd build

# Configure the project
cmake ..

# Build
make

# Run tests
ctest
```

## Configuration Options

The following CMake options are available:

- `CMAKE_BUILD_TYPE` - Set to either `Debug` or `Release` (default: `Release`)
- Add other project-specific options here

## Development

1. Place header files in `include/`
2. Place implementation files in `src/`
3. Add tests in `tests/`
4. Update CMakeLists.txt files as needed

## Testing

Tests are implemented using Catch2 and can be run using CTest. Test files should be placed in the `tests/` directory and named according to the pattern `test_*.cpp`.
