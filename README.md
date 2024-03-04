<div align="center">


<h1>ZenMode</h1>
<h2>规定时间内禁止打开App</h2>

</div>
<div align="center">


  [![Stars](https://img.shields.io/github/stars/Xposed-Modules-Repo/icu.insomnia.zen?label=stars)](https://github.com/Xposed-Modules-Repo/icu.insomnia.zen)
  [![LSP%20Repo](https://img.shields.io/github/downloads/Xposed-Modules-Repo/icu.insomnia.zen/total?label=LSP%20Repo&labelColor=F48FB1)](https://github.com/Xposed-Modules-Repo/icu.insomnia.zen/releases)[![Release](https://img.shields.io/github/v/release/Xposed-Modules-Repo/icu.insomnia.zen)](https://github.com/Xposed-Modules-Repo/icu.insomnia.zen/releases/latest)
</div>

<br/>

## preface
**此app仅修改`android.app.Activity#onResume`，不存在恶意代码，[源代码](https://github.com/People-11/FuckGJZS](https://github.com/NoonieBao/ZenMode))，请自行判断文件是否安全**

## Warning
确保你Xposed版本支持**作用域**，否则请勿安装<br/>
确保发生意外情况时您能够恢复设备！<br/>
推荐搭配`自动救砖`使用，[FuckGJZS](https://github.com/People-11/FuckGJZS)<br/>


## 使用步骤
1. 安装`app-release.apk`，并在Lsp作用域中勾选任何可能影响你的`app`
2. 在app中添加时间段即可。


## 增强

已察觉的某些关闭ZenMode的方式

| 种类        | 触发条件                  | Option                                   | 备注                                                         |
| ----------- | ------------------------- | ---------------------------------------- | ------------------------------------------------------------ |
| 唤起Lsp通知 | 安装新的模块唤起          | 勾选`应用包管理器`                       |                                        \*                          |
| 唤起Lsp通知 | 多开新的模块唤起          | 勾选`多开管理器`                         |                                               \*                   |
| 唤起Lsp     | 拨号唤起                  | 勾选`拨号界面`                           | 特殊命令可唤起Lsp，勾选拨号界面不影响接听来电。              |
| 唤起Lsp     | 快捷方式 \|\| Lsp寄生通知 | **先创建快捷方式，关闭通知，再移除通知** |                             \*                                     |
| 唤起magisk  |            \*               | 移除`Magisk图标`                         | 移除Magisk不会丢失权限，且不影响已授权应用。在想新授权时重新安装管理器即可。 |
| 文件管理器  |               \*                | 勾选`Root文件管理器`                     | Root文件管理器也可以移除增强模块。                           |

因此，可以对照上表进行设置以增强:
1. 通过Magisk将`ZenMode`升级为系统应用，这将使其不被卸载。（除非手动移除）
2. 勾选`拨号界面`，`应用包管理器`，`文件管理器`，`多开管理器`
3. 先初始化一次`Open Lsp Manger`授予`ZenMode`root权限(必须！，否则你可能无法手动打开Lsp)，按照上述表格方法移除Lsp通知和快捷方式。【可选】
4. 确保`ZenMode`正确被授权后，移除`Magisk快捷方式`，移除Magisk不会丢失权限，不影响已授权应用，在想新授权时重新安装管理器即可。【可选】
5. self-discipline batter than forced intervention



## 测试列表：

| phone        | API        | os              |
| ------------ | ---------- | --------------- | 
| K40 pro      | Android11  | MIUI12.5 12.5.8 |
| Xiaomi Note3 | Android 11 | crDroid 7.21    |
| MI 6         | Android 9  | MIUI10 9.9.3    |

在上述设备上测试通过


