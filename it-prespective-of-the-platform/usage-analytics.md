---
description: 通过数据，掌握规律
---

# 使用量分析

作为管理员，你随时可以查看整个公司使用Teams的统计数据，并且对其进行分析，以便掌握规律，帮助公司做出更好的决策。

## 通过管理中心查看并下载报告

通过登录到 [https://admin.teams.microsoft.com/analytics/reports](https://admin.teams.microsoft.com/analytics/reports) ，你可以进入“分析和报告“中心，在这里列出了常见的报表，如下图所示

![](../.gitbook/assets/tu-pian-%20%28182%29.png)

你还可以针对报表选择不同的日期范围，目前在管理中心支持：最近7天，最近30天，过去90天的数据。

{% hint style="warning" %}
不同的报表对应的日期范围选项可能不一样。
{% endhint %}

![](../.gitbook/assets/tu-pian-%20%28183%29.png)

点击“运行报表”按钮后，即可在线查看到所选报表的数据。

![](../.gitbook/assets/tu-pian-%20%28184%29.png)

如果你希望保存原始数据以便进一步分析（例如通过的图表展示），请点击上图中所示的 ”导出到Excel“ 按钮完成下载。

![](../.gitbook/assets/tu-pian-%20%28185%29.png)

点击上图中的 “下载” 按钮，即可得到一个CSV文件，其中就包含了当前报表的原始数据。

![](../.gitbook/assets/tu-pian-%20%28181%29.png)

通过管理中心查看报表进行分析非常方便

## 通过PowerShell脚本查看和下载报表



{% tabs %}
{% tab title="PowerShell" %}
```text
Install-Module Microsoft.Graph
```
{% endtab %}
{% endtabs %}



本节内容正在编写，敬请期待，您也可以订阅更新以便收到通知，或者基于现有内容提供反馈

{% page-ref page="../resource-of-the-book/how-to-follow-update.md" %}

导出报表结果

{% embed url="https://github.com/microsoftgraph/msgraph-sdk-powershell/issues/407" %}





