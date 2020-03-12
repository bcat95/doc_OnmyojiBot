工作原理
--------

文件结构
+++++++++

完整的文件就是这些::

    /onmyoji_bot文件夹
    ├── /img文件夹
    │   ├── /icon文件夹
    │   └── /screenshots文件夹
    ├── adb.exe
    ├── AdbWinApi.dll
    ├── AdbWinUsbApi.dll
    ├── CHANGELOG.md
    ├── Core.exe
    ├── ui.exe
    └── conf_example.ini

本工具的逻辑核心是 ``onmyoji.py`` ，编译后是 ``Core.exe`` （后面均以 ``onmyoji.py`` 指代这两个文件），没有图形界面。
所有的运行参数都是从 ``conf.ini`` 中读取。参数的详细说明可以参考 ``conf_example.ini`` 。

图形界面则是来源于 ``ui.py`` ，编译后是 ``ui.exe`` 用来生成配置文件 ``conf.ini`` 和调用执行 ``Core.exe``。

参数详解
+++++++++

下面结合UI以及 ``conf.ini`` 中所涉及到的配置参数，说明下每个参数是什么意义，在使用起什么作用。