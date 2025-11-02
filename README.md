# Hello World 示例项目

这个仓库包含使用 C 与 C++ 编写的经典“Hello, World!”示例程序，并提供了从构建到运行的完整说明，方便快速验证开发环境是否配置正确。

## 仓库结构

```
.
├── hello_world.c    # C 语言版本
├── hello_world.cpp  # C++ 版本
└── README.md        # 项目说明
```

## 环境准备

在大多数 Linux 或 macOS 发行版中，系统自带的编译器即可满足需求：

- C 语言：`gcc`
- C++ 语言：`g++`

如果你的系统尚未安装，可以在基于 Debian/Ubuntu 的系统上使用：

```bash
sudo apt update
sudo apt install build-essential
```

在基于 Fedora 的系统上可以使用：

```bash
sudo dnf groupinstall "Development Tools"
```

## 编译与运行

### 编译并运行 C 版本

```bash
gcc hello_world.c -o hello_world_c
./hello_world_c
```

### 编译并运行 C++ 版本

```bash
g++ hello_world.cpp -o hello_world_cpp
./hello_world_cpp
```

程序执行后，终端会输出：

```
Hello, World!
```

## 常见问题

- **找不到 `gcc` 或 `g++` 命令**：请先按照“环境准备”章节安装必要的工具链。
- **没有执行权限**：在某些系统上需要先赋予可执行权限，例如 `chmod +x hello_world_c`。

## 下一步

可以尝试修改程序，让它读取命令行参数或打印不同的信息，以熟悉编译与运行流程。

## 许可证

本项目仅用于学习与演示用途，欢迎自由复制与修改。
