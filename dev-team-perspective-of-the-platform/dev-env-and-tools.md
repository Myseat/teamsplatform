# 开发环境和工具

本节内容正在编写，敬请期待，您也可以订阅更新以便收到通知，或者基于现有内容提供反馈





## 安装PowerShell



## 使用 localhost.run 提供本地隧道功能



参考 [https://docs.microsoft.com/zh-cn/windows-server/administration/openssh/openssh\_install\_firstuse](https://docs.microsoft.com/zh-cn/windows-server/administration/openssh/openssh_install_firstuse) 的说明，在Windows 10中启用自带的OpenSSH 客户端。

将PowerShell 用管理员模式打开，通过下面的命令查看OpenSSH客户端的安装状态

```text
Get-WindowsCapability -Online | ? Name -like 'OpenSSH.Client*
```

在我的电脑上已经安装，会有如下的显示

![](../.gitbook/assets/tu-pian-%20%28267%29.png)





