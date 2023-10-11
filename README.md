# Valgrind Exercise
## Extra Credit 
- When the executable is linked statically, Valgrind shows more errors.
- It gives the conditional jump error but no memory leak.
- The reason could be that the executable, in this case, contains all the libraries instead of using them at just run time.
## Standard install via command-line
```bash
# Configure the project and generate a native build system:
  # Must re-run this command whenever any CMakeLists.txt file has been changed.
  cmake -S ./ -B build/
# Compile and build the project:
  # rebuild only files that are modified since the last build
  cmake --build build/
  # or rebuild everything from scracth
  cmake --build build/ --clean-first
  # to see verbose output, do:
  cmake --build build/ --verbose
# Run program:
  ./build/app/shell-app
# Clean
  cmake --build build/ --target clean
# Clean and start over:
  rm -rf build/
```

