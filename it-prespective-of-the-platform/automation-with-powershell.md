---
description: 使用脚本实现完全自动化
---

# 使用PowerShell 创建和管理团队

## 使用PowerShell 创建和管理团队

作为管理员，你也可以通过PowerShell 创建团队、频道、添加成员、安装应用，以便进行自动化或批量操作。下面是一些简单的范例。

{% hint style="info" %}
用PowerShell的方式可以实现比团队模板更加强大功能, 例如添加用户, 创建私有频道等.
{% endhint %}

### 连接到Microsoft Teams环境

```text
Import-Module MicrosoftTeams #非必须，但这样写是最保险的
Connect-MicrosoftTeams
```

### 创建团队

```text
New-Team -DisplayName "管理团队" -Description "通过PowerShell创建的团队" -OutVariable team
```

该命令会创建一个团队，并返回如下结果。请注意，默认团队是私有的。

![](../.gitbook/assets/tu-pian-%20%28290%29.png)

如果你想看这个团队的更多信息，可以用如下的命令。

![](../.gitbook/assets/tu-pian-%20%28287%29.png)

每个团队都有一个默认的频道，英文叫General，中文叫常规。

![](../.gitbook/assets/tu-pian-%20%28291%29.png)

### 创建频道

通过下面的命令可以为现有团队添加新的频道

```text
$team | New-TeamChannel -DisplayName "高管"
```

如果知道团队的编号，也可以用下面的方式添加

```text
New-TeamChannel -GroupId a2924e77-383a-4159-b231-0a3850f588eb -DisplayName "技术委员会"
```

而下面的命令是可以为团队添加私有频道

```text
$team | New-TeamChannel -DisplayName "私有频道" -MembershipType Private
```

### 添加成员

通过下面的命令可以为团队添加用户

```text
$team | Add-TeamUser -User panda@code365.xyz
```

或者

```text
Add-TeamUser -GroupId a2924e77-383a-4159-b231-0a3850f588eb -User tiger@code365.xyz
```

以上是把用户添加到团队, 如果需要将用户添加到私有频道, 你需要安装**预览版的PowerShell模块**

{% hint style="warning" %}
请注意, 安装多个版本可能会导致一些奇怪的问题. 我的做法是: 在PowerShell 7.1.x 这个最新版本PowerShell \(黑色\) 中安装正式版的模块, 在老的PowerShell \(蓝色, 版本号为5.1\) 中安装预览版.
{% endhint %}

```text
# 安装预览版的模块
Install-Module MicrosoftTeams -AllowPrerelease -RequiredVersion "2.2.0-preview"
```

请看清楚下面这个是我的蓝色PowerShell窗口

![](../.gitbook/assets/tu-pian-%20%28288%29.png)



### 为频道安装应用

### 修改团队设置

### 对团队进行归档



