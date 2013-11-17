---
layout: post
title: 环境变量
date: 2013-11-17 19:09
post-link: http://rgruet.free.fr/PQR27/PQR2.7.html#Environment
---

PYTHONHOME
: 替代的 *prefix* 目录（或 `prefix:exec_prefix`）。默认的模块搜索路径使用
  `prefix/lib`。

PYTHONPATH
: 增加模块文件的默认搜索路径。其格式与 Shell 的 `$PATH`
  相同。通过 `:` 或 `;` 来分隔一个或多个目录路径名称。

  替代的，你可以创建一个含有 `.pth` 扩展名的文本文件，每行一个路径，并将其置于
  Python 搜索路径的某处（理想之地是 `site-packages` 目录）。为每个应用程序创建
  `.pth` 较好，这样更易卸载。

PYTHONSTARTUP
: 如果是可读文件的名称，则该文件中的 Python 命令将在交互模式的第一个提示符显示
  前执行。

PYTHONDEBUG
: 若非空，则与 `-d` 选项相同。

PYTHONINSPECT
: 若非空，则与 `-i` 选项相同。

PYTHONOPTIMIZE
: 若非空，则与 `-O` 选项相同。

PYTHONUNBUFFERED
: 若非空，则与 `-u` 选项相同。

PYTHONVERBOSE
: 若非空，则与 `-v` 选项相同。

PYTHONCASEOK
: 若非空，则忽略文件/模块名的大小写（导入）。

PYTHONDONTWRITEBYTECODE
: 若非空，则与 `-B` 选项相同。

PYTHONIOENCODING
: 标准输入、标准输出及标准错误替代的 `encodingname` 或
  `encodingname:errorhandler`，与 `str.encode()` 接受相同的选择。

PYTHONUSERBASE
: 为用户指定的模块提供私有的 `site-packages` 目录。

PYTHONNOUSERSITE
: 若非空，则与 `-s` 选项相同。

PYTHONWARNINGS
: 允许控制警告，与 `-W` 选项相同。
