# oiutils

Fast and flexible programming contest manager of *zero* dependency.

(Recruiting someone to work on this project.)

## 工具集

* systools - 系统安装/初始化
* remote - 远程执行 (用于竞赛环境配置、收发文件、打包等)
* sched - 座位编排 & 约束求解
* sandbox - 沙盒运行
* judge - 文件比较 (容易配置灵活的 special judge)
* problem - 试题管理 (评测等，调用 fc, sandbox)
* contest - 竞赛评测生成报告 (调用 problem)

## 编程约定

* 最大程度兼容旧系统，使用 C++11 标准；
* Single binary，工具只有一个二进制文件；
* 可移植：尽可能使工具在 GNU 系统上可用；大部分功能在 Windows 下可用 (Cygwin)；
* Zero dependency: 不引入任何需要安装的库。如果的确需要，将代码导入到 repository 中。