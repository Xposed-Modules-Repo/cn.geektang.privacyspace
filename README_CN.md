## 隐秘空间

[![Stars](https://img.shields.io/github/stars/Xposed-Modules-Repo/cn.geektang.privacyspace?label=Stars)](https://github.com/GeekTR/PrivacySpace)
[![Release](https://img.shields.io/github/v/release/Xposed-Modules-Repo/cn.geektang.privacyspace?label=Release)](https://github.com/Xposed-Modules-Repo/cn.geektang.privacyspace/releases/latest)
[![Download](https://img.shields.io/github/downloads/Xposed-Modules-Repo/cn.geektang.privacyspace/total)](https://github.com/Xposed-Modules-Repo/cn.geektang.privacyspace/releases/latest)
[![Channel](https://img.shields.io/badge/Follow-Telegram-blue.svg?logo=telegram)](https://t.me/PrivacySpaceAlpha)
[![GitHub license](https://img.shields.io/github/license/Xposed-Modules-Repo/cn.geektang.privacyspace)](https://github.com/Xposed-Modules-Repo/cn.geektang.privacyspace/blob/main/LICENSE)

[源码](https://github.com/GeekTR/PrivacySpace)

这是一个**Xposed**模块。它可以将App“藏”起来，让其他App都找不到它们，可达到类似MIUI的“手机分身”功能。

## 它可以做到哪些很酷的事？

1. 某些银行类的App除了检测Root之外还会检测Xposed模块，它可以把我们的Xposed模块全藏起来，通过银行类App的检测；

2. 某个App的某个版本特别好用，我们不希望它被应用商店自动更新；

3. 我们在看广告的时候，某些App检测到另外的某个App的存在，会直接拉起，但是我们并不想打开这个被拉起的App；

4. 我们可能有某些学习软件不方便被别人看到，不然我们可能会很尴尬...；

5. 我们为什么要把安装了哪些App这么私人的事情告诉软件商家呢？

6. 更多更酷的事情等你发觉...

## 注意事项

1. 如果您的Magisk（面具）应用开启了随机包名功能，请将其加入白名单。否则移动至“隐秘空间”的APP将无法正确获取到Root权限；
2. 移动到“隐秘空间”的应用可以在“隐秘空间”主页面点击APP的图标启动；
3. ~~因为受限于系统，此APP需要Root权限才能正常工作~~（已不再需要）；
4. 如果不想对某个App隐藏（比如桌面），可以将其加入白名单；
5. 如果用此模块隐藏了一些系统APP，将可能导致重启后系统无法开机，请对系统应用谨慎操作；
6. 如果此模块导致您的系统无法启动，您可以在连接电脑后，在系统加载页面执行（开启usb调试的情况下）"adb uninstall cn.geektang.privacyspace"后再次重启。（或者您可以选择“搞机助手”的“自动神仙救砖”模块）。

## 待办事项

计划实现以下功能。

- [x] 应用列表页面新增搜索功能
- [x] 适配Android 8-10
- [x] 移除对Root权限的依赖
- [ ] 配置备份与恢复
- [ ] 安装Xposed模块自动隐藏（用户可选）
- [ ] 隐藏Xposed模块时由用户自行选择是否加入其推荐APP为其关联应用

## 作用域

1. Android系统（**必选**）

2. 勾选非Android系统作用域时可对进行针对性hook（勾选Android系统后隐藏功能不能对其生效时使用）
