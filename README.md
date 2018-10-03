![Java快速编译工具](http://upload-images.jianshu.io/upload_images/13775732-a537d606fea4ddb0?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
# Java快速编译工具使用手册

---
**适用范围：**快速编译较为简单的Java源程序
**开发人员：**强力发明狂
**下载地址：**https://github.com/cambridgejames/Java_Fast_Compiler.git
---
### 程序说明
**说明：**本程序为针对较为简单的Java项目进行快速编译的轻量级小程序，目的在于将初学者从命令行编译中解放出来。
**优点：**本程序在不需要用户手动敲击CMD命令的同时，在用户点击编译、运行等按钮时，会自动生成相应的CMD命令并通过对话框显示出来供用户确认，在方便用户编译的同时也可加深用户对编译具体操作的理解。
**运行环境：**本程序的原理为调用JDK和JRE，故需要用户自行安装Java集成开发环境（JDK）。同时，虽然本程序自带了部分动态链接库，但在部分计算机中仍可能需要手动安装Microsoft Visual C++ 2015运行库。

---
### 操作手册
##### 1. 编译Java源文件
启动Java快速编译工具，界面如下图1.1所示：
![图1.1 Java快速编译工具界面](http://upload-images.jianshu.io/upload_images/13775732-76f32e1778532c75?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
点击“**源代码存储路径**”右侧的“**浏览…**”按钮，在打开的对话框中选择Java源文件主类所在的文件目录，如下图1.2所示：
![图1.2 选择Java源文件所在的目录](http://upload-images.jianshu.io/upload_images/13775732-80e406979b9b9c40?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
单击右下角的“**确定**”按钮。此时，字节码文件的目标存储路径会默认变为与源代码存储路径一致，如图1.3所示。
![图1.3 Java字节码文件存放的目录](http://upload-images.jianshu.io/upload_images/13775732-bf46401bc05a745c?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
点击“**字节码文件目标存储路径**”右侧的“**浏览…**”按钮，在打开的对话框中选择字节码文件即将存放的目录，如下图1.4所示：
![图1.4 选择Java字节码文件存放的目录](http://upload-images.jianshu.io/upload_images/13775732-1158277dadf2a1c8?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
单击右下角的“**确定**”按钮。
在“**包名、主类名及参数**”编辑框中填写主类的类名称，如下图1.5所示：
![图1.5 填写Java主类名称](http://upload-images.jianshu.io/upload_images/13775732-d1732ab4530696bf?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
在“**文件编码格式**”下拉选项中选择Java源文件的编码格式。编码格式默认为UTF-8，但也可以选择其他的编码格式，如下图1.6所示：
![图1.6 选择Java源文件的编码格式](http://upload-images.jianshu.io/upload_images/13775732-3aad6869f94d37f5?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
设置完成后，点击右侧的“**编译**”按钮，程序将弹出对话框确认即将执行的CMD命令，点击“**是**”则执行该命令，点击“**否**”则取消当前操作，返回主界面继续修改设置，如下图1.7所示：
![图1.7 确认即将执行的CMD命令](http://upload-images.jianshu.io/upload_images/13775732-31bb42ec357233ca?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
若点击“编译”按钮后出现如图1.8所示的错误提示，则说明之前的设置有误，需要点击“**确定**”按钮返回主界面，修改编译设置后重新进行编译。
![图1.8 编译设置错误](http://upload-images.jianshu.io/upload_images/13775732-25824d39263c40fd?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
成功开始编译后，若编译通过，则程序主界面底部的编辑框中显示“编译成功”，如图1.9及1.10所示，程序将会之前设置的字节码文件目录中生成相应的字节码文件。否则程序主界面底部的编辑框中将会显示相应的错误信息，如图1.11所示。
![图1.9 编译成功界面](http://upload-images.jianshu.io/upload_images/13775732-a3bfe6e5549594d5?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![图1.10 新生成的字节码文件](http://upload-images.jianshu.io/upload_images/13775732-1b826a19d3932327?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![图1.11 编译失败后的错误提示](http://upload-images.jianshu.io/upload_images/13775732-b025cd0c5fe020e9?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

##### 2. 运行Java字节码文件
启动Java快速编译工具，界面如下图2.1所示：
![图2.1 Java快速编译工具界面](http://upload-images.jianshu.io/upload_images/13775732-b6a648b44563665e?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
点击“**字节码文件目标存储路径**”右侧的“**浏览…**”按钮，在打开的对话框中选择编译Java源文件时选择的字节码文件存放的目录，如下图2.2所示：
![图2.2 选择Java字节码文件存放的目录](http://upload-images.jianshu.io/upload_images/13775732-5ce3975d7a793188?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
单击右下角的“**确定**”按钮。
在“**包名、主类名及参数**”编辑框中填写“(包名.(包名.(...)))主类名(参数)”。若无包名和参数，则可只填写主类名，如下图2.3所示：
![图2.3 填写包名、主类名及参数](http://upload-images.jianshu.io/upload_images/13775732-add2096a8e377e75?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
设置完成后，点击右侧的“**运行**”按钮，程序将弹出对话框确认即将执行的CMD命令，点击“**是**”则执行该命令，点击“**否**”则取消当前操作，返回主界面继续修改设置，如下图2.4所示：
![图2.4 确认即将执行的CMD命令](http://upload-images.jianshu.io/upload_images/13775732-322bb3d241b6e508?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
若点击“是”，则程序将启动CMD窗口并执行设置路径中的Java程序，程序执行完毕后CMD窗口不会消失，如图2.5所示。若CMD窗口出现闪退，则可能是前一步设置有误，需要用户自行排查错误。
![图2.5 程序的执行结果](http://upload-images.jianshu.io/upload_images/13775732-d17d75dd2d88d4ea?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

##### 3. 手动编译Java源文件
除自动编译外，本程序也支持用户手动输入CMD命令进行编译，具体步骤如下：
启动Java快速编译工具，界面如下图3.1所示：
![图3.1 Java快速编译工具界面](http://upload-images.jianshu.io/upload_images/13775732-febf650bcab6b2fb?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
点击“**源代码存储路径**”右侧的“**浏览…**”按钮，在打开的对话框中选择Java源文件主类所在的文件目录，如下图3.2所示，然后单击右下角的“**确定**”按钮将路径填入编辑框。
![图3.2 选择Java源文件所在的目录](http://upload-images.jianshu.io/upload_images/13775732-f787a39f64752325?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
点击程序主界面左侧的“**启动CMD**”按钮，程序将弹出对话框确认即将执行的CMD命令，点击“**是**”则执行该命令，点击“**否**”则取消当前操作，返回主界面继续修改设置，如下图3.3所示：
![图3.3 确认即将执行的CMD命令](http://upload-images.jianshu.io/upload_images/13775732-9e5f0d6066084656?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
若点击“是”，则程序将启动CMD窗口并自动切换至Java源程序所在的目录，如图3.4所示。
![图3.4 CMD窗口](http://upload-images.jianshu.io/upload_images/13775732-5fcbc38e64033d1a?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
**注：**本实用说明中的全部源代码及字节码文件保存在“**程序安装目录\demo**”文件夹下。

---
若程序在使用中出现任何问题，请联系程序开发人员：

**ID：**强力发明狂
**邮箱：**cambridge_james@foxmail.com
**QQ：**1412244189
**微博：**@强力发明狂

---
版权所有 &copy; copyright 2018
