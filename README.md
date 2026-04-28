# HarmonyOSComponentUXExamples 项目说明

## 一、项目简介
本项目是基于HarmonyOS ArkTS（Stage模型）开发的UI组件示例集合，包含多种ArkUI常用组件的用法与交互实现，用于鸿蒙应用开发的学习与作业提交。

## 二、项目目录结构说明

HarmonyOSComponentUXExamples-master/
├── .hvigor/              # Hvigor构建工具的配置与缓存目录
├── .idea/                # DevEco Studio IDE的配置文件（不影响项目运行）
├── AppScope/             # 应用全局配置目录，存放应用级资源与配置
├── entry/                # 应用主模块（核心业务代码目录）
│   ├── build/            # 编译生成的产物目录（无需提交到Git）
│   ├── config/           # 模块级配置文件，包含编译、签名等配置
│   └── src/              # 模块源码目录
│       └── main/ets/     # ArkTS业务代码目录，Index.ets为应用主入口页面
├── screenshots/          # 项目运行截图、演示资源目录
├── .gitignore            # Git忽略文件配置，指定无需提交的文件/目录
├── build-profile.json5   # 应用编译构建的全局配置文件
├── hvigorfile.ts         # Hvigor构建工具的项目入口脚本
├── oh-package.json5      # 项目依赖管理文件，声明项目依赖的组件与版本
└── README.md             # 项目说明文档（即本文件）

## 三、核心文件说明
 1.  **`entry/src/main/ets/Index.ets`**
     项目主入口页面，用`@Entry`声明为应用启动页，包含页面生命周期`aboutToAppear()`和UI构建`build()`方法，实现了导航栈+列表的动态布局。
 2.  **`oh-package.json5`**
     鸿蒙项目的依赖管理文件，类似前端的`package.json`，声明项目所需的ArkUI组件库、API版本等依赖信息。
 3.  **`build-profile.json5`**
     应用全局配置文件，包含应用包名、版本号、签名配置、模块信息等，是鸿蒙应用打包运行的核心配置。
 ## 四、运行说明
 1.  开发环境：DevEco Studio + 对应版本的HarmonyOS SDK
 2.  运行方式：在DevEco Studio中打开项目，同步依赖后，可在模拟器或鸿蒙真机上运行，查看各UI组件的示例效果。