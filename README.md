# jshint for sublime 配置及使用方法 v1.0.7
### 安装：npm install-TopuNet-JsHint4Sublime  

文件结构：
-------------

		1. .jshintrc 放入项目根目录

使用：
--------------

1. node.js>npm install -g jshint
1. 在sublime安装package：JSHint
1. 将 “npm目录\jshint.cmd” 加入到系统环境变量Path中

        如：C:\Users\Administrator\AppData\Roaming\npm\jshint.cmd
1. 打开js文件
1. Alt + j
1. 正常显示：

            [JSHint: 当前文件路径]

            ✓ 0 errors, [esc] to hide.

            [Finished in 0.5s]

1. 错误显示：

            [JSHint: 当前文件路径]

              20,28: Expected an assignment or function call and instead saw an expression.
              20,34: Missing semicolon.

            ✗ 2 errors, double-click above, [F4] for next, [shift-F4] for previous.

            [Finished in 0.4s]

            此时双击具体错误行，可以快速跳转至错误所在行

注意：
--------------

1. 每次进行验证前，需要将修改保存，否则还是在检测旧版本的代码。
1. .jshintrc可以记录忽略项。如遇忽略项有添加，可以直接 pull request 到github上。
1. 解决不了的问题需要上报。

更新记录：
--------------
v1.0.7

        1. 增加忽略项：EXIF
        
v1.0.6

        1. 增加忽略项：WeixinJSBridge和JRoll
        
v1.0.5

        1. 增加忽略项：fis
        
v1.0.4

        1. jshintrc文件增加expr规则（是否允许上下文为表达式），为true。——苏成闯 pull

v1.0.3

        1. 从jshintify转到jshint
        2. 修改Readme

v1.0.2

        1. 增加忽略项：process、module
        2. 修改忽略项数组的排序，以后查找方便

v1.0.1

        创建项目并发布
