---
layout: post
title: 调用选项
date: 2013-11-17 18:01
post-link: http://rgruet.free.fr/PQR27/PQR2.7.html#Invocation
---

    python[w] [-BdEhimOQsStuUvVWxX3] [-c command | scriptFile | - ] [args]

-B
: 阻止从创建的 `.pyc` 或 `.pyo` 文件导入模块（参阅环境变量
  `PYTHONDONTWRITEBYTECODE=x` 及属性 `sys.dont_write_bytecode`）

-d
: 输出解析器的调试信息（参阅 `PYTHONDEBUG=x`）

-E
: 忽略环境变量（如 `PYTHONPATH`）

-h
: 打印帮助信息并退出（原来是 `-?`）

-i
: 在执行脚本后进入交互式解释器，即使 `stdin`（标准输入）未出现于终端，也强制产生
  提示符（参阅 `PYTHONINSPECT=x`）

-m module
: 在 `sys.path` 中搜索模块，并将模块作为脚本执行（2.5 中的改进实现：`runpy`
  模块）

-O
: 优化生成的字节码（参阅 `PYTHONOPTIMIZE=x`）。断言被抑制

-OO
: 除 `-O` 优化外还移除了 `doc-strings`（文档字符串）

-Q arg
: 除法选项：`-Qold`（默认）、`-Qwarn`、`-Qwarnall`、`-Qnew`

-s
: 禁用用户指定的模块路径（参阅 `PYTHONNOUSERSITE=x`）

-S
: 在初始化时不执行 `import site`

-t
: 对不一致的 Tab 用法发出警告（`-tt`：发出错误）

-u
: 不带缓存的二进制 `stdout`（标准输出）和`stderr`（标准错误）（参阅
  `PYTHONUNBUFFERED=x`

-U
: 强制 Python 将所有字符串字面量作为 Unicode 字面量解释

-v
: 冗余输出（跟踪导入语句）（参阅 `PYTHONVERBOSE=x`）

-V
: 打印 Python 版本号并退出

-W arg
: 警告控制（`arg` 是 `action:message:category:module:lineno`）

-x
: 跳过源代码的第一行，允许使用 `#!cmd` 的非 Unix 形式

-3
: 对 `2to3` 无法修复的 Python 3.x 不兼容性发出 `DeprecationWarning`

-c command
: 指定要执行的命令。这将终结选项列表（跟着的选项作为参数传给命令）

scriptFile
: 要执行的 Python 文件（`.py`）名称。从标准输入读取

-
: 从标准输入读取程序（默认，如果是 tty 则进入交互模式）

args
: 传给脚本或命令（在 `sys.argv[1:]` 中）


: 如果无 scriptFile 或命令，Python 则进入交互模式
