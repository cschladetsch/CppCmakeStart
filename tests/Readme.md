# Tests

This directory contains the project's test suite using Catch2 framework.

## Organization

- Test files should be named `test_*.cpp`
- Each component should have its own test file
- Group related tests using TEST_CASE and SECTION

## Running Tests

Tests can be run using CTest:
```bash
cd build
ctest
```

Or run specific test executables directly:
```bash
./build/bin/test_component_name
```

## Writing Tests

1. Use meaningful test names that describe the behavior being tested
2. Follow the Arrange-Act-Assert pattern
3. Test both normal and edge cases
4. Keep tests independent and isolated
5. Use appropriate fixtures for setup/teardown

## Test Coverage

The project can be configured to generate test coverage reports using gcov/lcov:

```bash
cmake -DCMAKE_BUILD_TYPE=Debug -DENABLE_COVERAGE=ON ..
make
make coverage
```

Coverage reports will be generated in `build/coverage/`.
