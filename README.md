# Ninja

Ninja是一个注重速度的小型构建系统。
https://ninja-build.org/

有关背景和更多详细信息,请参见发行版中所包含的[手册](https://ninja-build.org/manual.html)或[文档](doc/manual.asciidoc).

Linux，Mac和Windows的二进制文件位于[GitHub](https://github.com/ninja-build/ninja/releases).
运行`./ninja -h`以获得更多帮助信息.

不需要进行安装，因为唯一需要的文件是生成的Ninja二进制文件.
但是,要启用Bash补全,Emacs和Vim编辑模式等功能,`misc/`中的某些文件必须复制到适当的位置.

如果您想对Ninja进行更改，请先阅读[CONTRIBUTING.md](CONTRIBUTING.md).

## Building Ninja itself

您可以通过使用Python编写的脚本或通过CMake编译Ninja,有关更多详细信息,请参见[wiki](https://github.com/ninja-build/ninja/wiki).

### Python

```
./configure.py --bootstrap
```

### CMake

```
cmake -Bbuild-cmake -H.
cmake --build build-cmake
```

运行以下命令以进行测试:

```
./build-cmake/ninja_test
```
