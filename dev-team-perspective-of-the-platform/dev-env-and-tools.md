# 开发环境和工具

本节内容正在编写，敬请期待，您也可以订阅更新以便收到通知，或者基于现有内容提供反馈





## 安装PowerShell

作为开发人员，你经常需要访问Microsoft Teams的数据，以便进行验证和自动化。PowerShell将会让你事半功倍。

建议安装最新的7.1.3或者更高版本，这是一个跨平台的版本。请通过 [https://docs.microsoft.com/zh-cn/powershell/scripting/install/installing-powershell?view=powershell-7.1](https://docs.microsoft.com/zh-cn/powershell/scripting/install/installing-powershell?view=powershell-7.1) 进行安装，并安装 `MicrosoftTeams` 这个模块，以及 `Microsoft.Graph` 和`Az` 这两个模块 （可选，但推荐）。

```text
Install-Module MicrosoftTeams,Microsoft.Graph,Az
```

## 创建开发证书提供https支持



## 使用 ngrok 提供本地隧道功能

在很多微软的官方文档中都提到了 `ngrok` 这个工具，这可能是目前用的最广泛的一个将本地网站发布到外网，并且默认提供https支持的服务。它的官方网站是 [https://ngrok.com/](https://ngrok.com/) 。

ngrok 有免费版和收费版，也有多种安装方式。请参考这里的说明：[https://ngrok.com/download](https://ngrok.com/download)。我自己比较喜欢的方式是将其作为npm的全局模块安装，如下

```text
npm install -g ngrok
```

这样做的好处就是可以直接用 ngrok 命令

## 使用 localhost.run 提供本地隧道功能

ngrok很不错，但我还发现另外一个更加轻量级的方案（localhost.run\)， 它有永久免费的版本，甚至不需要安装专门的客户端，而是使用标准的SSH 客户端即可。

首先请 参考 [https://docs.microsoft.com/zh-cn/windows-server/administration/openssh/openssh\_install\_firstuse](https://docs.microsoft.com/zh-cn/windows-server/administration/openssh/openssh_install_firstuse) 的说明，在Windows 10中启用自带的OpenSSH 客户端。

将PowerShell 用管理员模式打开，通过下面的命令查看OpenSSH客户端的安装状态

```text
Get-WindowsCapability -Online | ? Name -like 'OpenSSH.Client*
```

在我的电脑上已经安装，会有如下的显示

![](../.gitbook/assets/tu-pian-%20%28270%29.png)

如果可以通过如下的命令进行安装

```text
Add-WindowsCapability -Online -Name OpenSSH.Client~~~~0.0.1.0
```

一切准备就绪！假设你本地开发的项目，在 localhost:3000 运行，你可以使用下面的命令来建立一个隧道

```text
ssh -R 80:localhost:3000 localhost.run
```

很快你看到如下的输出，表示创建隧道成功了

![](../.gitbook/assets/tu-pian-%20%28264%29.png)

访问这个https的地址，它会把请求转发到本地的网页。

![](../.gitbook/assets/tu-pian-%20%28260%29.png)

{% hint style="warning" %}
请注意，免费版的地址是随机生成的。如果你需要固定的地址，请访问 https://admin.localhost.run 进行设置。
{% endhint %}

