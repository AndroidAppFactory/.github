[ ![Github](https://img.shields.io/badge/bihe0832-AndroidAppFactory-brightgreen?style=social) ](https://github.com/bihe0832/AndroidAppFactory)
[ ![Github](https://img.shields.io/github/last-commit/bihe0832/AndroidAppFactory) ](https://github.com/bihe0832/AndroidAppFactory)
[ ![Github](https://img.shields.io/github/stars/bihe0832/AndroidAppFactory?style=social) ](https://github.com/bihe0832/AndroidAppFactory)
[ ![Github](https://img.shields.io/bitbucket/issues/bihe0832/AndroidAppFactory) ](https://github.com/bihe0832/AndroidAppFactory)

## 关于 AAF

做酱油的时候发现做开发那么久竟然没有一整套顺手的开发方案，要从头开始一个一个搭建（相当于之前做的就没什么沉淀），因此开始逐渐整理一整套相对全面并且顺手的开发方案。随着这几年逐渐完善，现在基本上具备雏形了，因此逐渐总结一下。

AAF 是基于组件化方案，逐渐积累的一套 Android 终端开发方案。方案力求做到**技术方案可以轻松的从一个项目复用到另一个项目，或者可以快速在框架基础上开发出一个独立全新的应用**，开发过程中基本聚焦在新业务的逻辑，而不是基础功能。

## 框架介绍

这是AAF的一个总体架构：

![](https://android.bihe0832.com/doc/aaf_architecture.png?v=1)

整个AAF框架共有四层：

- **基础组件**：基础组件 `Router*` 是路由相关的基础组件，`Lib*` 是自己沉淀或者统一对比以后选择的第三方技术栈，**与业务无关，可通用**。

- **公共组件**：基础框架 `Framework` 负责通用资源、公共声明、页面路由以及对于底层第三方库的二次封装，所有业务通用的基础通用功能。`Common*` 则是聚焦一个具体的业务无关的功能，例如反馈、内置浏览器等，这部分功能**也与业务无关，可通用**。

- **业务组件**：基础框架 `Application` 包含与业务相关的一些公共资源定义，基础功能封装等。`Base*` 则是聚焦一个具体的业务功能，例如页面卡片、广告等。

- **应用组件**：应用组件是可以独立运行的最小单元，而且他们基本只是一个Android Application 的空壳加一些配置文件，所有的业务逻辑都在业务组件层实现。其中里面比较特别的是APPTest，他既是底层业务组件开发中的临时入口，同时也是一些基础功能 和 所有 Pub的测试入口。
<!--
## 主要代码

<a href="https://github.com/AndroidAppFactory/AndroidAppFactory"><img src="https://github-readme-stats.vercel.app/api/pin?username=AndroidAppFactory&repo=AndroidAppFactory" width ="45%" /></a> <a href="https://github.com/AndroidAppFactory/AndroidAppFactory-Sample"><img src="https://github-readme-stats.vercel.app/api/pin?username=AndroidAppFactory&repo=AndroidAppFactory-Sample" width ="45%" /></a>

<a href="https://github.com/AndroidAppFactory/Template_Android"><img src="https://github-readme-stats.vercel.app/api/pin?username=AndroidAppFactory&repo=Template_Android&v1" width ="45%" /></a> <a href="https://github.com/AndroidAppFactory/Template-AAF"><img src="https://github-readme-stats.vercel.app/api/pin?username=AndroidAppFactory&repo=Template-AAF" width ="45%" /></a>

-->
## 相关链接

## 相关链接

- **框架使用：**

    - **运行Demo**：[https://android.bihe0832.com/doc/sample/start.html](https://android.bihe0832.com/doc/sample/start.html)
	
    - **使用框架独立开发**：[https://android.bihe0832.com/doc/sample/customize.html](https://android.bihe0832.com/doc/sample/customize.html)
	
- **框架文档：**

    - 链接：[https://android.bihe0832.com/doc/](https://android.bihe0832.com/doc/)
    
    - 内容：主要**介绍相关组件的功能以及整体框架使用相关的内容**

- 技术方案介绍：

    - 链接：[https://blog.bihe0832.com/android-dev-summary.html](https://blog.bihe0832.com/android-dev-summary.html)
    
    - 内容：完整AAF的整个技术方案，以及其中一些核心的技术点
	
- 代码统计：

   - 框架代码：[https://android.bihe0832.com/source/lib/index.html](https://android.bihe0832.com/source/lib/index.html)

   - AAF Sample 代码：[https://android.bihe0832.com/source/sample/index.html](https://android.bihe0832.com/source/sample/index.html)


