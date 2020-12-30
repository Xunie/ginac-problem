# Using GiNaC as a git submodule -- example

## How to build

```bash
git clone --recursive git://github.com/Xunie/ginac-problem.git
cd ginac-problem
mkdir -p _build
cd _build
cmake -GNinja -DCMAKE_BUILD_TYPE=RelWithDebInfo ..
cmake --build .
```
