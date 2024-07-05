## Windows 使用配置

[toc]

Windows 10





### 键盘

按键设置

- 如何改键：
  1. 使用 Windows PowerToys
  2. AutoHotKey
  3. 注册表 Keyboard Layout



> Windows PowerToys 的按键映射对部分组合键不支持，如 Windows + L，详细查看：[适用于 Windows 的 PowerToysKeyboard Manager 实用工具 | Microsoft Learn](https://learn.microsoft.com/zh-cn/windows/powertoys/keyboard-manager#keys-that-cannot-be-remapped)



> 注册表使用Scancode Map的方式，但windows没有提供相应的文档，详细可以查看：[Where can I find Windows keyboard scancode registry information? - Super User](https://superuser.com/questions/550679/where-can-i-find-windows-keyboard-scancode-registry-information)



按键替换：

带有 `Home` 和 `End` 键会比较方便

> 没有 `Home` 或 `End` 的电脑一般使用 `Fn` 和左右方向键的组合。

1. 中文英文使用环境中 `Caps Lock` 的使用频率不高，设置为 `F5`；也可以通过 `Caps Lock` 键扩展功能；
2. `Alt_R` 设置为 `Win`；
2. `Ctrl_R` 设置为 `F2`， 常用于重命名；



> *Alt_R 指键盘右侧的Alt键，Alt_L 指键盘左侧的Alt键，其余同理







注册表 reg 文件

```reg
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layout]
"Scancode Map"=hex:00,00,00,00,00,00,00,00,02,00,00,00,5c,e0,38,e0,00,00,00,00
```









### 鼠标

中键(滚轮按键) -> Ctrl+W

用于网页等程序的快速关闭，结合Shift键可强制关闭(并非所有程序有用)



前进键 -> Win

仅在隐藏任务栏且无法通过鼠标移动唤出的情况下(如使用task homie)推荐使用，用于仅通过鼠标唤出

> 1. 相对而言后退键的使用更加频繁，故不替换后退键
> 2. Edge可以通过手势控制(右键按住划，需要在设置中开启)实现前进







### 触控板

windows中叫触摸板

在设置中可以调整，结合使用选择

触摸板-高级手势配置



1. 三指上划/下滑 -> 放大/缩小窗口
2. 三指右划 -> 切换窗口
3. 三指左划 -> 仅显示当前窗口
4. 三指点按 -> Ctrl + W
5. 四指点按 -> Alt + F4
6. 四指左划/右划 -> 切换桌面
7. 四指上划 -> 操作中心
8. 四指下滑 -> Win





### Edge

手势控制：

仅建议使用如下四种手势：

|           |           |
| --------- | --------- |
| 向左/向右 | 前进/后退 |
| 向上      | 全屏切换  |
| 向下      | 新建窗口  |
|           |           |

触控板：

双指拖动

前进 & 后退

放大 & 缩小



Vimium C：

|      |      |
| ---- | ---- |
|      |      |











### 软件

PowerToys

Task Homie





输入法控制

Weasel

|                  |                    |      |
| ---------------- | ------------------ | ---- |
| Ctrl+Space       | 禁止输入法         |      |
| Ctrl+Shift+Space | Weasel内输入法切换 |      |
|                  |                    |      |
| Win+Space        | 系统输入切换       |      |





### 输入法

小鹤双拼



