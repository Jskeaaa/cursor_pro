# Cursor增强工具

之前的已经失效，现在可以用我的cursor-pro-max.exe这个工具这里面的卡号可以绑cursor，地址随机生成就好了。国内ip就可直接绑卡，我的项目里有教程。但不短时间不能频繁绑卡，会封ip（切勿乱用，有问题可以给我issues）

## 主要功能

* **重置机器码** - 通过生成随机的机器ID来重置Cursor的使用限制
* **突破Claude 3.7 Sonnet限制** - 启用高级功能，突破免费版限制
* **清理Cursor应用数据** - 清理历史记录和缓存文件，包括:
  * 删除 `globalStorage/state.vscdb` 和 `globalStorage/state.vscdb.backup` 文件
  * 清空 `History` 文件夹内的所有内容
  * 删除 `workspaceStorage` 文件夹及其内容
* **终止Cursor进程** - 快速关闭所有Cursor相关进程

## 问题解决

当遇到以下问题时，本工具可以帮助解决：

<img src="ee959738cc1fe045a8e741b906a100fb.png" alt="问题实例" width="400"/>

> **注意**: 当操作后仍遇到限制时，可能是IP被污染，建议更换IP后再尝试（已经有少部分用户出现这种情况）。可多尝试几次重置操作。

## 使用指南

### Windows系统

#### 图形界面版本

1. 下载最新的`cursor_enhance_tool.zip`并解压
2. 右键点击`cursor_enhance_tool.exe`，选择"**以管理员身份运行**"
3. 在弹出的图形界面中选择需要的功能：
   - 重置机器码
   - 突破Claude 3.7 Sonnet限制
   - 清理Cursor应用数据
   - 终止Cursor进程

#### 命令行版本（旧版）

1. 右键点击`cursor_clean.exe`，选择"**以管理员身份运行**"
2. 按照命令行提示选择操作选项

### Mac系统

#### 使用Python脚本

1. 打开终端(Terminal)
2. 进入脚本所在目录
3. 执行以下命令运行脚本:
```
sudo python3 cursor_clean_mac.py
```

> **注意**：在Mac系统中程序需要管理员权限才能运行，因为需要访问系统受保护的文件。


## 配置文件

### Windows系统

程序会自动创建 `config.env` 配置文件，您可以根据需要修改其中的路径设置：

```ini
[PATHS]
# Cursor用户数据目录路径
base_path = C:\Users\用户名\AppData\Roaming\Cursor\User
```

配置文件需要和可执行文件放在同一目录。

### Mac系统

程序会自动创建 `config_mac.env` 配置文件，您可以根据需要修改其中的路径设置：

```ini
[PATHS]
# Cursor用户数据目录路径
base_path = ~/Library/Application Support/Cursor/User
```

配置文件需要和脚本或可执行文件放在同一目录。



## 免责声明

本工具仅用于学习和研究目的，请勿用于商业用途。使用本工具产生的任何问题由用户自行承担。请在使用前备份重要的Cursor配置。
