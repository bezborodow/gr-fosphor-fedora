# gr-fosphor-fedora

Fosphor

https://projects.osmocom.org/projects/sdr/wiki/Fosphor



https://github.com/osmocom/gr-fosphor



Compilation error when Qt is disabled?

`/home/dbezborodov/src/gr-fosphor/python/bindings/qt_sink_c_python.cc:15:10: fatal error: QWidget: No such file or directory
15 | #include <QWidget>`

Needed packages:

```
glfw glfw-devel glfw-doc
intel-opencl mesa-libOpenCL mesa-libOpenCL-devel  opencl-headers
cmake
gnuradio-devel
spdlog-devel
libmpc-devel
opencl-headers mesa-libOpenCL-devel intel-opencl-clang-devel rocm-opencl-devel
freetype-devel
pybind11-devel
swig
qt5-qtbase-devel
```

Then set up the library path:

```
sudo sh -c 'echo /usr/local/lib64 > /etc/ld.so.conf.d/local-x86_64.conf'
sudo ldconfig
```
