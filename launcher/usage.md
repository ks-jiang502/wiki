# SakuraFrp 启动器基本使用指南

## 安装启动器 {#install}

登录管理面板，转到 **软件下载** 页面：

![](../_images/download.png)

选择 **启动器**，点击右侧下载按钮下载启动器安装程序：

![](./_images/usage-0.png)

::: tip
如果在安装过程中碰到问题，请参阅 [启动器常见安装问题](/faq/launcher#install)
:::

下载完毕后运行安装程序并根据向导提示进行安装：

![](./_images/usage-1.png)

通常情况下一直点 **下一步** 即可，您也可以参考下图选择需要安装的功能：

![](./_images/usage-1.5.png)

## 登录启动器 {#login}

::: tip
传统启动器和新版 (WPF) 启动器使用方法基本一致，此处仅提供新版启动器的教程
:::

安装完毕后双击桌面图标 (如果您选择了 `创建桌面快捷方式`) 来运行启动器。

::: tip
如果您没有勾选 `创建桌面快捷方式`，请打开 `C:\Program Files\SakuraFrpLauncher` 文件夹，然后运行 `SakuraLauncher.exe`  (如果安装的是传统启动器，请运行 `LegacyLauncher.exe`)  
![](./_images/usage-2.png)
:::

进入 [用户信息](https://www.natfrp.com/user/profile ':target=_blank') 页面，复制 **访问密钥** 到启动器，点击 **登录**：

![](./_images/usage-3.png)

## 创建隧道 {#create-tunnel}

::: tip
启动器的创建隧道功能相对简陋，我们推荐您到 [SakuraFrp 管理面板](https://www.natfrp.com/user/) 创建隧道以获得更好的使用体验
:::

登录成功后会自动切换到 **隧道** 标签，点击加号新建隧道：

![](./_images/usage-4.png)

::: tip
本文档提供了 HTTP、RDP 等常见应用的配置指南，请查看左侧边栏的 **常见应用配置指南** 列表
:::

接下来选择您要映射的服务，此处以映射 `iperf3` 服务器为例，直接找到进程 `iperf3` 点击，然后选择一个服务器，最后点创建即可：

![](./_images/usage-5.png)

创建成功后按需要选择是否继续创建：

![](./_images/usage-6.png)

## 启用隧道 {#start-tunnel}

::: tip
不要频繁开关隧道，启用隧道后稍等一会才能连接成功。如果长时间 (超过一分钟) 没看到连接成功的提示框请检查日志
:::

在隧道标签中找到您要启用的隧道，点击右上方开关启用

![](./_images/usage-7.png)

启动成功后右下角会弹出通知，提示隧道连接方式。该通知可以在设置中通过 `关闭隧道状态提示` 选项禁用

![](./_images/usage-8.png)

转到日志标签可以复制连接方式

![](./_images/usage-9.png)

这样我们的服务就可以在外网被访问到了

![](./_images/usage-10.png)

## 删除隧道 {#delete-tunnel}

将鼠标放到隧道卡片上悬停一会，卡片右上角会出现删除按钮

![](./_images/usage-11.png)

点击删除按钮，然后确认操作即可删除隧道

![](./_images/usage-12.png)

## 开机启动 {#autostart}

`2.0.0.0` 及以上版本的启动器提供两种开机启动方式，一般情况下直接勾选下图中的选项就能满足使用需求

如需不进桌面自启 (如穿透远程桌面服务)，请参阅 [系统服务](/launcher/service) 页面了解服务启动方式

![](./_images/usage-13.png)
