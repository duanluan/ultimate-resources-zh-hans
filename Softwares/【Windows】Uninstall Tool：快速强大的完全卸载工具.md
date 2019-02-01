![](https://www.crystalidea.com/assets/images/uninstall-tool/logo-320.png)

# 简介

强大的卸载工具，卸载不需要的软件，使你的计算机更加干净、快速。

## 卸载向导

启动卸载向导后，清理残留文件。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_wizard.png)

### 延迟删除

当系统正在使用文件或文件夹时，会在下次 Windows 重新启动时删除。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_wizard_delayed_removal.png)

### 检测并终止正在运行的进程

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_wizard_terminate_process.png)

### 详细的删除日志

卸载完成时，你可以查看/保存详细的删除日志。删除日志记录了每个操作（例如尝试删除文件/文件夹/注册表或终止进程/取消注册 COM 对象等）。操作失败时，会在日志中添加相应的错误代码和说明。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_wizard_removal_log.png)

## 跟踪安装

安装应用程序时，会跟踪对系统所做的所有更改。

### 如何跟踪安装

可以通过 3 种方式完成：

![文件右键菜单](https://www.crystalidea.com/assets/images/uninstall-tool/screen_monitor_context_menu.png)
![底部工具栏](https://www.crystalidea.com/assets/images/uninstall-tool/screen_monitor_toolbar.png)
![Windows 任务栏图标菜单](https://www.crystalidea.com/assets/images/uninstall-tool/screen_monitor_taskbar.png)

跟踪安装后，如果所有进程都已完成，将自动停止跟踪，否则你必须在安装完成后手动停止。

成功安装后，新程序将显示在列表中，并带有“已跟踪”标记，在卸载过程中将删除所有跟踪数据（在卸载向导中）。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_monitor_traced_mark.png)

### 安装进度

在跟踪安装时，会最小化到系统托盘。你可以通过双击托盘图标或托盘上下文菜单来查看实时进度。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_monitor_progress.png)

你可以使用还原功能停止跟踪安装：

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_monitor_revert.png)

### 安装多个程序

安装跟踪器能检测和处理这种情况：安装完成后，显示已安装列表，并允许用户选择主要程序。列表标记主要程序为“已跟踪”，并将其它程序视为相关程序。卸载一个跟踪程序时，也会删除相关程序的跟踪数据，并且会显示警告消息。

### 附加数据

需要配置或者更新新版本时。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_monitor_append.png)

指定一个可执行文件，安装跟踪器将继续跟踪并附加新数据。

## 强制删除

使用卸载向导查找和删除程序，不运行关联卸载程序。

卸载向导会对残留文件和注册表进行深层扫描，它能够找到并删除 Windows 服务（包括驱动程序）、文件关联、COM 组件（包括 Shell 扩展）和各种 Windows Installer 相关组件、快捷方式等痕迹。

当要卸载的应用程序某些进程正在运行时，卸载向导会提示终止它们。

卸载已跟踪的应用程序时，卸载向导会显示跟踪列表，达到最佳效果。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_force_removal_wizard.png)

## 批量删除

按住 Ctrl 逐个选择需要删除的程序（或按住 Shift 使用键盘上/下键选择相邻程序）。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_batch.png)

**批量强制删除痕迹**不会运行关联卸载程序，只会扫描残留并合并到列表中。

**批量从列表中删除项目**仅从列表中删除项目，而不删除所选程序的任何文件、注册表。请谨慎使用此功能，仅用于删除过时或者无效的列表条目。

**批量卸载**目前仅限于卸载 Windows 应用商店应用。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_batch_wizard.png)

## 自启动项

启用/禁用或删除在 Windows 启动时启动的任何应用程序。

检测无效条目。

查看每个条目的详细信息（安装文件夹、发布者、命令行、状态和来源）。

批量操作所选项目（使用 Ctrl 选择多个程序）。

定期查看启动应用程序列表（以及删除不需要的项目）时优化 PC 启动性能的好方法。此外，你可以及时检测秘密安装在你计算机上的各种间谍软件/广告软件。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_startup.png)

### 启动类型

卸载工具检测通过以下方式启动的程序：

* HKLM Run - HKEY_LOCAL_MACHINE 注册表项，所有计算机用户。
* HKLM RunOnce - HKEY_LOCAL_MACHINE 注册表项，所有计算机用户。此项目仅启动一次。
* HKCU Run - HKEY_CURRENT_USER 注册表项。
* HKCU RunOnce - HKEY_CURRENT_USER 注册表项。此项目仅启动一次。
* StartMenu All - 所有用户的开始菜单、启动文件夹（通常是开始菜单\程序\启动）。
* StartMenu CU - 当前用户的开始菜单、启动文件夹。
* Windows Task - 在用户登录时的 Windows 任务。你还可以添加新的计划任务。

### 添加新的启动程序

你可以添加一个新程序，该程序将在 Windows 启动时自动启动。启动类型可以是上面列表中的任何类型。

* **启动类型** - 程序启动的方式，请参考上面的列表。
* **可执行文件路径** - 你要启动的程序的可执行文件完整路径。
* **参数**（可选） - 你希望为程序指定的命令行参数列表。
* **以最高权限运行任务** - （仅适用于 Windows 任务）以管理员身份运行。

## 便携版

无需安装即可使用其所有功能。

随身携带（U 盘）其设置和许可证，就可以在任何 Windows 计算机上使用。

程序缓存和跟踪安装数据仍位于本地计算机上。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_portable.png)

### 便携版和跟踪安装

便携版也可以完全正常运行跟踪安装，但是使用跟踪安装程序时不能通过“文件右键菜单”打开。

![](https://www.crystalidea.com/assets/images/uninstall-tool/screen_monitor_toolbar.png)

### 便携版许可证

注册数据会保存到文本文件“license.dat”中，该文件放在程序文件夹中。

文件内容：

第一行 - 注册名称

第二行 - 注册码

例：

John Smith

KGT4-YGRT-GHTR-7G31

# 资源

|名称|资源名|地址|备注|
|---|---|---|---|
|Uninstall Tool|官网|[Uninstall Tool](https://www.crystalidea.com/uninstall-tool)||
||便携版下载地址|[Portable version download link](https://www.crystalidea.com/downloads/uninstalltool_portable.zip)||
||注册码|[uninstall Toole 注册码_百度搜索](https://www.baidu.com/s?wd=uninstall+Toole+%E6%B3%A8%E5%86%8C%E7%A0%81)||
||破解版|[uninstall Toole 破解版_百度搜索](https://www.baidu.com/s?wd=uninstall+Toole+%E7%A0%B4%E8%A7%A3%E7%89%88)||
