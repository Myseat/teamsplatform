---
description: 两大方向，六种能力，三个范围
---

# 平台能力一览

## 概述

Microsoft Teams 平台支持两个方向的定制或集成开发，分别是：

1. 通过**定制和扩展Teams客户端**（不管是桌面端还是移动端），将你的应用场景跟Teams原生的界面结合起来，让广大的用户可以在一个集中的入口（Teams客户端中），完成更多的工作。
2. 将Teams的能力，**通过接口的方式，整合到你的应用系统**中去。这个是借助于已经很成熟的Microsoft Graph这个能力来实现的。

这两个方向都很重要，本书都会详细介绍。在定制和扩展Teams客户端这个角度，合作伙伴或开发人员可以将一个或者多个能力用一个“应用（Teams App）” 的概念进行定义，除去Microsoft Graph这个能力外，其他的五个能力分别是:

1. 选项卡
2. 机器人
3. 消息扩展
4. 连接器
5. 通知

并且进行分发和管理，并且可以安装到三个不同的层面（范围）。

1. 个人层面
2. 团队层面
3. 会议层面

## Teams 客户端扩展点和功能集

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>&#x80FD;&#x529B;</b>
      </th>
      <th style="text-align:left"><b>&#x4E2A;&#x4EBA;</b>
      </th>
      <th style="text-align:left"><b>&#x9891;&#x9053;</b>
      </th>
      <th style="text-align:left">
        <p><b>&#x9891;&#x9053;</b>
        </p>
        <p><b>&#x804A;&#x5929;</b>
        </p>
      </th>
      <th style="text-align:left"><b>&#x5355;&#x804A;</b>
      </th>
      <th style="text-align:left"><b>&#x7FA4;&#x804A;</b>
      </th>
      <th style="text-align:left">
        <p><b>&#x4F1A;&#x8BAE;</b>
        </p>
        <p><b>&#x804A;&#x5929;</b>
        </p>
      </th>
      <th style="text-align:left"><b>&#x4F1A;&#x8BAE;</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">&#x9009;&#x9879;&#x5361;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x2714;</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x673A;&#x5668;&#x4EBA;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x6D88;&#x606F;&#x6269;&#x5C55;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">&#x67E5;&#x8BE2;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">&#x64CD;&#x4F5C;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">&#x94FE;&#x63A5;&#x89E3;&#x6790;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">&#x8FDE;&#x63A5;&#x5668;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Office 365&#x8FDE;&#x63A5;&#x5668;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Incoming webhook</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Outgoing webhook</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">&#x901A;&#x77E5;</td>
      <td style="text-align:left">&#x2714;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>

## Microsoft Graph 能力一览表

利用Microsoft Graph 所提供的API, 你可以拥有Teams完整生命周期的管理能力，也就是说，你可以把Teams的功能集成到现有应用中去。

![](../../.gitbook/assets/tu-pian-%20%2810%29.png)

这个功能列表还在不断的增加，现在的接口已经有几十个之多了。

![](../../.gitbook/assets/tu-pian-%20%2811%29.png)

有意思的是，要使用Microsoft Graph的这些强大能力，你也需要定义一个“应用程序（Application）“来实现，并且申请对应的权限。但这个应用程序是指在Azure AD中定义的一个对象，与上面提到的Teams App是完全不同的概念。

如何定义和开发应用会在后续的章节展开，接下来先给大家介绍一些上述提到六种能力的典型场景。

