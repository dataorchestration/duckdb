1) clone the duckdb 
2) cd duckdb
3) git clone https://github.com/duckdb/duckdb.git 
4) cd duckdb
5) mkdir build
6) cd build
7) this will create makefiles in duckdb folder```shell
cmake -DCMAKE_BUILD_TYPE=Release \
      -DBUILD_EXTENSIONS="arrow" \
      -DBUILD_ARROW_EXTENSION=ON \
      -DBUILD_SHELL=ON \
      -DCMAKE_VERBOSE_MAKEFILE=ON \
      ..
```
8) cd ..
9) make -j8