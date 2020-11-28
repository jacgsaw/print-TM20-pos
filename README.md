Instalacion y configuracion de impresoras post en 80mm, 58mm aunque esta medida es personalizable desde el archivo .c

Para compilar el ejecutable correctamente solo hay que seguir lo que dice el manual.

You need toolchain, CMake and cups-devel.

It may be achieved, say (as example) by running
```
sudo apt install build-essential cmake libcups2-dev libcupsimage2-dev
```

Also if you want to build own PPD it is highly desirable to have available `ppdc` compiler.
Build is done out-of-the source.

```
  mkdir build && cd build && cmake /path/to/source
  cmake --build .
```
