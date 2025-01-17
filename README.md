## rvcc

本课程基于Rui的[chibicc](https://github.com/rui314/chibicc)，@sunshaoce和@ksco将其由原来的X86架构改写为RISC-V 64架构，同时加入了大量的中文注释，并且配有316节对应于每一个commit的课程，帮助读者可以层层推进、逐步深入的学习编译器的构造。

- 课程对应的代码仓库位于：https://github.com/sunshaoce/rvcc
- 课程对应的视频课程位于：https://space.bilibili.com/296494084

### 前提要求
需要一定的C编程能力，不要求编译原理相关的知识。

需要具有一个Linux系统环境，推荐Ubuntu 20.04。同时安装RISC-V相关环境：clang、qemu-riscv64（相关视频参考：https://www.bilibili.com/video/BV1D54y1m78G ）。

### 构建
项目的构建命令为：`make`。

（可选）项目使用CMake的构建命令为：
```shell
cmake -Bbuild .
cd build/
make
```

### RISC-V介绍
RISC-V是一个开源的精简指令集，相较于常见的X86、ARM架构，其简单易学，并且发展迅猛。现在已经出现了支持RISC-V的各类设备，未来还将出现RISC-V架构的笔记本电脑，可谓是前景一片光明。

### chibicc

[chibicc](https://github.com/rui314/chibicc)是Rui开发的一个X86架构的迷你编译器。Rui同时也是8cc、9cc、mold、lld等著名项目的主要开发者，chibicc是他最新的编译器项目。chibicc项目以commit为阶段，借助于316个commits实现了一个能够编译Git等项目的C编译器，同时层层深入的课程，也大大降低了难度，帮助更多人来上手chibicc。
