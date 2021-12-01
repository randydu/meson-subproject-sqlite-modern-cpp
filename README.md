# meson subproject for [sqlite modern cpp](https://github.com/SqliteModernCpp/sqlite_modern_cpp.git)

Our version matches the latest release version v3.2 of the sqlite-modern-cpp lib. 


## Usage

- Step 1: copy "sqlite-modern-cpp.wrap" to the "subprojects" folder of your main project;
- Step 2: in the main project's meson.build:

```meson
# import
sqlite_modern_cpp_dep = dependency('sqlite-modern-cpp')

# use

srcs = ['main.cpp', ...]
executable('test', srcs, dependencies: [sqlite_modern_cpp_dep, ...])
```

in your source code:

```c++
#include <sqlite_modern_cpp.h>

```