# 概念

## Tools

* 编辑器
  * 输入处理“文本”，可能有拓展功能，如智能提示、代码高亮、智能格式化
  * VSCode

* 编译器
  * 将源代码变成二进制文件、可执行文件（包含预处理、编译、汇编、连接四步）
* 集成开发环境
  * 包括编辑器、编译器、调试器图形用户界面工具
  * Dev C++、Visual Studio、Charm、Keil、STM32CubeIDE

## 源代码变为可执行程序的四步

* 预处理（生成 .i 的临时文件)
  * 删除所有的注释、宏拓展、文件包含
* 编译（ .i 转换成 .s 的汇编语言文件)
* 汇编（ .s 转换成 .o 的机器码文件)
* 链接（ .o 转换成 .exe 的可执行文件）

## 终端

* 定义：与计算机交互的界面
* 功能：接受用户输入并将结果输出给用户
* 当下的交互界面
  * GUI（图形用户界面）（主要，但早期不存咋）
  * Terminal（终端） （早期交互方式）
* 存在多种类型的终端（每个终端都有不同的功能和特点）
  * CMD（Command Prompt）：Windows自带
  * PowerShell：微软开发（除了 CMD 外，Windows 还提供了其他几种终端，例如 PowerShell 和 Windows Terminal）
  * Bash
  * ucrt64

## 初始化配置VSCodeC语言环境相关概念

* **MinGw-w64**
  * 开源的编译器和工具集
  * 属于MSYS2的一部分
  
* **MSYS2**
  * 工具和库的集合,一个开源软件包管理系统
  * 为 GCC、mingw-w64、CPython、CMake、Meson、OpenSSL、FFmpeg、Rust、Ruby 等提供最新的原生构建
  * 由名为mintty的命令行终端\Bash\如Git和Subversion的版本管理系统\如tar和awk工具组成提供
  * Pacman包管理系统:提供便捷包的安装\更新方法
  
* **CMake**（本身不带编译功能）

  * 本质: 定义各个目标的关联(构建工具的本质)

    * 比如项目由哪些可执行文件\动态库\资源文件组成, 又是通过哪些源文件编译,  用到了哪些外部关联等
    * 是一种描述构建过程的脚本语言，不是传统的编程语言

  * 功能: **自动化**完成多组件\源代码文件的编译\链接\打包形成; 还可以添加单元测试; 创建安装包; 将功成拆分成若干个子目录更利于大型项目的管理

    * 单一源代码文件----无需工程文件
    * 略微复杂含库\多源代码文件的项目----可以手动配置工程文件

  * CMakeLists.txt:

    * 自己写的构建规则, 用来描述项目结构和构建逻辑
    * 基本使用CMake命令写，而非函数

  * 

  * **配置(Configure)**: CMake根据CMakeLists.txt生成**原生工程文件**; 生成bin文件夹中的exe文件

    * 原生工程文件

      * 如Windows下的VS工程\Linux下的Makefile
      * >原生: 专门为某一特定操作系统或硬件平台设计的应用程序或组件
        >
        >工程文件: 用于组织和管理项目, 包含了项目的配置信息

  * **构建(Build)**: 生成build文件夹中的配置相关文件
  
  * <img src="C:\Users\33071\Pictures\Screenshots\屏幕截图 2024-08-15 214549.png" style="zoom:75%;" />

# C语言的工程规范

## 多文件

* 代码复用: 将常用函数卸载一个文件中
* 代码结构清洗
* 编译速度快: 只有修改的文件需要重新编译, 不需要每次都编译整个项目

## 规范的工程模板

* bin文件夹: 可执行文件 (.exe)
* build文件夹: 编译过程中生成的文件
* lib文件夹: 库文件
* docs文件夹: 文档
* inc文件夹: 头文件 (.h文件)
* src文件夹: 源文件 (如.c文件)
* CMakeLists.txt: CMake的配置文件|Makefile: Make的配置文件
* README.md: 项目说明

## 编程规范

* 清晰第一: 一般情况下, 可读性比性能更重要
* 简洁为美: 长代码难以看懂, 容易在修改时引入错误; 废弃代码(没有调用的函数和全局变量)要及时清除; 重复代码应该尽可能提炼成函数
* 选择合适的风格, 与代码原有风格保持一致

## 头文件规范

* 头文件只包含函数声明|宏定义|结构体生命|全局变量生命等, 不包含函数定义
* 头文件中不要包含其他头文件, 只包含当前文件需要的头文件
* 头文件中不要定义全局变量, 全局变量应在.c文件中定义❓(全局变量定义和声明的区别)
* 头文件中不要定义宏, 宏应该在.c文件中定义
* 要记得加上**头文件保护宏**, 防止头文件被重复包含

## 函数规范

* 一个函数只做一件事，同时函数的名字要能够有效地体现出函数的功能。
* 重复代码应该尽可能提炼成函数。
* 避免函数过长，新增函数不超过50行(非空非注释行)。
* 避免函数的代码块嵌套过深，新增函数的代码块嵌套不超过4层。

## 变量规范:question:

* 变量名要有意义，不要使用无意义的变量名，如a、b、c等。
* 变量名要尽量简洁，同时要能够有效地体现出变量的含义。
* 变量名要使用小写字母，单词之间使用下划线分隔(也可以是驼峰式命名，如：addItem、isChineseStudent 等)。
* 变量名要尽量避免使用缩写，除非是广泛使用的缩写。
* 不用或者少用全局变量，全局变量会增加代码的耦合性，使代码难以维护。
* 防止局部变量与全局变量同名。
* 明确全局变量的初始化顺序，避免跨模块的初始化依赖。

## 注释规范

* 注释要写在需要解释的代码上方或右侧，而不是下方。
* " // " 和 " /* " 后要有一个空格。
* 大段注释使用 "/**/" ，小段注释使用 " // "
* 一个函数的注释应该包括函数的功能、输入参数、输出参数、返回值等

![](C:\Users\33071\Pictures\Screenshots\屏幕截图 2024-08-15 221508.png)

> 推荐插件: **Prettier**

# Makefile & CMake

# 版本管理与代码协作

* git: 是一个免费的、开源的分布式版本控制系统，可以高速处理从小型到大型的各种项目。
* 版本控制：是一种记录文件内容变化，以便将来查阅特定版本修订情况的系统。

<img src="C:\Users\33071\AppData\Roaming\Typora\typora-user-images\image-20240815223901200.png" alt="image-20240815223901200" style="zoom:100%;" />

![v2-d715a963f0378a226181df321d03f112_r](C:\Users\33071\Desktop\v2-d715a963f0378a226181df321d03f112_r.jpg)

![image-20240822115539384](C:\Users\33071\AppData\Roaming\Typora\typora-user-images\image-20240822115539384.png)





- [ ] 将.vscode文件夹从33071中移到Coding-related-tools文件夹中, 在VSCode中所有拓展显示未下载, 而.vscode文件夹中有一个.extension文件夹 
  * .xxxxxxx文件夹代表的是正常情况隐藏的文件夹(可以在文件资源管理器中更改设置)
  * .xxxxxxx文件夹一般是通常用于存储应用程序的配置、缓存或者其他用户不需要直接访问的数据。它们的存在是为了避免干扰用户的日常操作，同时又能让应用在后台正确运行
  * 在移动或处理这类文件夹时，请谨慎操作，因为它们可能包含应用程序的重要数据。如果你不确定某个文件夹的作用，最好不要随意移动或删除它，以免影响到对应的应用程序。
- [ ] 如何避免CMake在每次更改后都会重新编译修改文件，会很影响电脑性能吗
- [ ] 一个奇怪的现象: nodejs作为拓展包, 下面还有拓展包, 具体层次如下

* nodejs
  * StandardJS
  * Prettier ESLint
  * Surround
  * SVG
  * svelte
    * Svelte for VS Code
    * Svelte Intellisense
    * Svelte 3 Snippets
* C/C++
* Prettier - Code formatter
* React
* PlatformIO IDE
* Go
* CMake Tools
* C/C++ Themes
* CMake
* C/C++ Extension pack
* Chinese

<img src="C:\Users\33071\Pictures\Screenshots\屏幕截图 2024-08-02 114043.png" alt="Extensions" style="zoom:25%;" title="Extensions"/>

- [ ] github上存储的项目如何跳转渲染成网页

<img src="C:\Users\33071\Pictures\Screenshots\屏幕截图 2024-08-08 113300.png" style="zoom:25%;" />





### CMake 的特点:

- **脚本语言**: CMakeLists.txt 文件是基于文本的脚本文件，类似于 Shell 脚本。
- **非图灵完备**: CMake 不是一种图灵完备的语言，这意味着它没有循环、条件语句等传统编程语言的全部功能。
- **配置文件**: CMakeLists.txt 文件更像是配置文件，而不是程序代码。
- **命令式**: CMake 使用一系列预定义的命令来描述构建过程。

### CMake 的组成部分:

- **命令**: CMake 提供了一系列内置命令，如 `add_executable`, `add_library`, `install` 等，用于描述构建过程。
- **函数**: 用户可以定义自己的函数来封装一系列命令，实现更复杂的功能。
- **变量**: 可以设置和使用变量来存储和传递信息。

### 与其他语言的关系:

- **与 C/C++ 的关系**: CMake 主要用于构建 C 和 C++ 项目，但它也支持其他语言，如 Java、Python 等。
- **与脚本语言的关系**: CMake 类似于脚本语言，但它的设计目标更侧重于构建过程的描述，而不是通用的编程。

CMake构建及安装指令

```
mkdir build && cd build
cmake .. -DCMAKE_INSTALL_PREFIX=./local
make
make install
```

CMakeList.txt模板

```cmake
cmake_minimum_required (VERSION 3.10)

project (test)

set (EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)

#SRC_LIST为生成exe文件必须变量，两种赋值方式
#SET（SRC_LIST 源文件名）
#aux_source_directory (指定根目录下的某一目录为搜索目录 SRC_LIST)
aux_source_directory (src SRC_LIST) 

include_directories (inc)

add_executable (test ${SRC_LIST})
```

