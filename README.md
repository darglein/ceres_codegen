# Standalone Ceres code generation example

Build instructions:

- Clone the ceres patch from https://ceres-solver-review.googlesource.com/c/ceres-solver/+/16341/
- Run CMake with -DCODE_GENERATION=ON
- Build and install Ceres
- Build and run this sample

## Tested Configurations

Platform | Compiler | INSTALL | EXPORT_BUILD_DIR 
--- | --- | --- | --- 
Linux | gcc | :heavy_check_mark: | :heavy_check_mark:
MacOS | clang | TODO | TODO
Windows | msvc | TODO | TODO
