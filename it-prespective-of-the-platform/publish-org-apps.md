# 发布和管理企业应用

## 审核自定义应用

Microsoft Teams 允许普通用户在需要时向管理员提交自定义应用，以便在公司更加广泛地使用。

![](../.gitbook/assets/tu-pian-%20%28215%29.png)

用户提交应用后，管理员在“管理应用” 这个界面，可以看到有等待审批的应用的数量，请在下面的列表中，点击一下“发布状态”这个列标题，可以快速看到哪些是 “已提交”状态的应用。

{% hint style="warning" %}
用户提交后，管理员不会收到通知。这个功能有待改进。
{% endhint %}

![](../.gitbook/assets/tu-pian-%20%28233%29.png)

点击该应用的名称，在应用的详情页面中，查看该应用的更多信息，并且决定改如何处理。

![](../.gitbook/assets/tu-pian-%20%28216%29.png)

将发布状态修改为 “发布” 意味着你批准并发布它，用户将能够在应用商店中看到这个应用。

![](../.gitbook/assets/tu-pian-%20%28220%29.png)



## 购买第三方应用

在Microsoft Teams官方市场中，有几百个各种各样的第三方应用，虽然绝大部分都是免费的，但也有一部分是需要收费才能使用的。目前，在美国市场上面，Teams 允许管理员集中地为员工购买授权。详情请参考下面的介绍。

{% embed url="https://docs.microsoft.com/zh-cn/MicrosoftTeams/purchase-third-party-apps" %}

这个功能还是很有必要的，用户需要更好的应用，而合作伙伴也需要有正常的商业收入，让我们期待这方面的生态和体系越来越好。

## 自定义第三方应用

这个同样是还没有完全开放的功能，就是支持对一个第三方应用进行自定义（主要是对名称，图标等信息），使得其更加容易被本公司员工使用。

毫无疑问，要进行这样的自定义，必须是该应用的开发者设置了允许自定义才行。目前这个功能，还处于“开发者预览” 阶段，也就是说，只有使用“开发者预览” 这个架构文件（schema）定义的应用，才支持这个特性，管理员也才能进行后续自定义。

下面是一个简单的例子。这个json文件是用来定义应用清单信息的，首先必须使用 [https://raw.githubusercontent.com/OfficeDev/microsoft-teams-app-schema/preview/DevPreview/MicrosoftTeams.schema.json](https://raw.githubusercontent.com/OfficeDev/microsoft-teams-app-schema/preview/DevPreview/MicrosoftTeams.schema.json) 这个schema，同时manifestVersion必须设置为devPreview，此时你可以定义configurableProperties 的信息。

```javascript
{
  "$schema": "https://raw.githubusercontent.com/OfficeDev/microsoft-teams-app-schema/preview/DevPreview/MicrosoftTeams.schema.json",
  "manifestVersion": "devPreview",
  "version": "1.0.1",
  "isFullScreen": true,
  "id": "b9614c28-aa31-4d7e-b67c-4c08a0036699",
  "packageName": "sample.teamsdev.cod365",
  "developer": {
    "name": "Code365.xyz",
    "websiteUrl": "https://teamsplatform.code365.xyz",
    "privacyUrl": "https://teamsplatform.code365.xyz",
    "termsOfUseUrl": "https://teamsplatform.code365.xyz"
  },
  "icons": {
    "color": "color.png",
    "outline": "outline.png"
  },
  "name": {
    "short": "平台手册",
    "full": "平台手册"
  },
  "description": {
    "short": "平台手册范例应用",
    "full": "平台手册范例应用"
  },
  "accentColor": "#FFFFFF",
  "staticTabs": [
    {
      "entityId": "teamsplatformguide",
      "name": "主页",
      "contentUrl": "https://teamsplatform.code365.xyz",
      "scopes": ["personal"]
    },
    {
      "entityId": "about",
      "scopes": ["personal"]
    }
  ],
  "permissions": ["identity", "messageTeamMembers"],
  "validDomains": ["teamsplatform.code365.xyz"],
  "configurableProperties": [
    "name",
    "longDescription",
    "shortDescription",
    "largeImageUrl",
    "smallImageUrl"
  ]
}

```

目前支持自定义的属性一共有几个，分别如下

* `name`：允许管理员更改应用显示名称。
* `shortDescription`：允许管理员更改应用的简短说明。
* `longDescription`：允许管理员更改应用的详细说明。
* `smallImageUrl`：它是 `outline` 清单 `icons` 块中的 属性。
* `largeImageUrl`：它是 `color` 清单块 `icons` 中的 属性。
* `accentColor`：它是要与 和 一起使用的颜色，作为大纲图标的背景。
* `developerUrl`：它是 https:// 网站的 URL。
* `privacyUrl`：它是 https:// 隐私策略的 URL。
* `termsOfUseUrl`：它是 https:// 使用条款的 URL。

只要是这样定义的应用，不管是发布到了官方商店，还是提交到公司的商店，它的“可自定义” 这一列会变成 "是”，选中此应用时，工具栏中的 “自定义”按钮就可以使用，管理员可以上述提到的属性进行自定义。

![](../.gitbook/assets/tu-pian-%20%28242%29.png)

{% hint style="danger" %}
很遗憾，在写作本文时，我可以修改这个manifest，但无法上传，所以无法完成实际上的截图。该问题已经在反馈处理中。
{% endhint %}

## 自定义应用商店





