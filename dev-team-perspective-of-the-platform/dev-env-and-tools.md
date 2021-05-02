# 开发环境和工具

本节内容正在编写，敬请期待，您也可以订阅更新以便收到通知，或者基于现有内容提供反馈





## 安装PowerShell

建议安装最新的7.1.3或者更高版本，这是一个跨平台的版本。请通过 [https://docs.microsoft.com/zh-cn/powershell/scripting/install/installing-powershell?view=powershell-7.1](https://docs.microsoft.com/zh-cn/powershell/scripting/install/installing-powershell?view=powershell-7.1) 进行安装，并安装 `MicrosoftTeams` 这个模块，以及 `Microsoft.Graph` 和`Az` 这两个模块 （可选，但推荐）。

```text
Install-Module MicrosoftTeams,Microsoft.Graph,Az
```

## 使用 ngrok 提供本地隧道功能



## 使用 localhost.run 提供本地隧道功能



参考 [https://docs.microsoft.com/zh-cn/windows-server/administration/openssh/openssh\_install\_firstuse](https://docs.microsoft.com/zh-cn/windows-server/administration/openssh/openssh_install_firstuse) 的说明，在Windows 10中启用自带的OpenSSH 客户端。

将PowerShell 用管理员模式打开，通过下面的命令查看OpenSSH客户端的安装状态

```text
Get-WindowsCapability -Online | ? Name -like 'OpenSSH.Client*
```

在我的电脑上已经安装，会有如下的显示

![](../.gitbook/assets/tu-pian-%20%28268%29.png)

如果可以通过如下的命令进行安装

```text
Add-WindowsCapability -Online -Name OpenSSH.Client~~~~0.0.1.0
```

一切准备就绪，假设你本地开发的项目，在 localhost:3000 运行，



