---
description: 微软历史上成长速度最快的应用
---

# Microsoft Teams 及其发展

我在本书的序言中提到 Microsoft Teams 出现的一些背景信息。2016年左右，微软的Office 365 已经取得初步的成功，作为公司核心的三朵云之一，服务于越来越多的企业客户，包括很多从传统的Office Server，以及本地客户端升级过来的客户。

> Microsoft Azure, Office 365, Dynamics 365 是当时的三驾马车，现在Office 365这个品牌已经升级为 Microsoft 365， 另外还要加上Power Platform这第四朵云。

熟悉微软的朋友们可能知道，这次起源于2010年前后的向云转型的过程，是一次充满未知的巨大冒险。当时的情形大致是，Windows 和 Office 一如既往取得了不错的成绩，但在搜索、互联网、社交、移动入口等这些领域面临的挑战也是前所未有的。

向云转型并不容易，对微软来说也有利有弊。构建云计算平台和服务需要大量基础建设，前期投入非常大，短期内可能见不到经济效益。好在微软本身有很强大的技术底蕴，和忠实的客户群体。现在回过头去看看Office 365一路走过来的过程，我总结是有三个主要的阶段：

1. 云化
2. 服务化
3. 平台化

**云化是第一步**。微软有非常成功的Office客户端软件家族，以及多个企业级服务产品（Exchange Server，SharePoint Server，和 Lync Server—— 后来改名为 Skype for Business Server），那么既然要做云中的Office，就需要把这些软件都搬到云端去吧。有条件咱要上，没有条件咱创造条件也要上啊。

技术上说，这个阶段的目标就是整合上面提到的三个服务器产品，加上Office Online Server，让用户可以通过一个账号就能访问这些服务，并且无缝地沟通和协作。这是SasS服务的早期阶段，对终端用户来说，其实感受的变化不是很大，因为除了账号少了一些，服务还是那些服务，该怎么操作还是要怎么操作。但对于信息管理部门来说则已经意味着改变，安装和维护服务器不再是日常的主要工作，规划和管理用户及授权，合理分配资源，在效能和安全之间取得平衡等等成为了新的话题。

![](../.gitbook/assets/image%20%2813%29.png)

**服务化是必然趋势**。Office 365既然是SaaS应用，就要体现出来“软件即服务——Software as a Service”的特点，其中一个基本的要求就是，它所提供的能力，最好能以颗粒度更小的形式提供，并且允许客户自己的需求进行组合购买，仅为它购买的那部分服务付费。这个阶段把一些模块从三大服务组中分离出来，例如OneDrive for Business，Videos就是一个非常成功的例子，与此同时推出了更多全新的服务，包括本书的主角Microsoft Teams，以及下面列出的这些服务（仅为部分）。

![](../.gitbook/assets/image%20%2814%29.png)

**平台化的战略和两大抓手**。作为一个云服务，Office 365 用户日常使用会产生大量的数据，如何让这些数据能被客户自身（或通过可信的合作伙伴）加以利用甚至跟客户自身的应用进行整合呢？微软在2015年的build大会上，正式发布了Microsoft Graph 这个服务，通过一个统一的地址（[https://graph.microsoft.com](https://graph.microsoft.com)），使用最流行的REST API（以及各种SDK）的方式可以方便并且安全地访问这些有价值的数据。这是Office 365走向平台的一个重要举措，Microsoft Graph 作为平台在云端能力的一种集中体现，但微软似乎还需要一个能够广泛触达到用户的应用，并且支持合作伙伴或用户直接基于这个应用进行定制或扩展，实现更多价值。

> 2015年宣布Microsoft Graph的视频在这里 [https://channel9.msdn.com/Events/Build/2015/KEY01](https://channel9.msdn.com/Events/Build/2015/KEY01)

![](../.gitbook/assets/image%20%2810%29.png)



我想，Microsoft Teams 就是在这样的大背景下诞生的。一方面，用户需要有更加现代的沟通协作体验，Skype for Business作为传统的企业级应用，功能相对有限无法满足用户的需求，也很难跟市场上新出现的一些对手做竞争。另外，Office 365有那么多服务，各种客户端，如何集中起来为用户提供平台服务，和Microsoft Graph搭档起来，从云+端（Cloud+Edge\) 两个角度形成一套完整的平台？这个使命，至少目前看来，是落在了Microsoft Teams身上了。

即便是如此，从Microsoft Teams 面世第一天开始，也伴随着各种疑问，其中被客户问的最多的问题就是：Office 365已经有Outlook，Skype for Business等全系列产品可以做沟通与协作，那么Teams 的具体定位是什么呢？

![](../.gitbook/assets/image%20%2815%29.png)











Teams 和其他产品的关系

Teams 发布以来的主要业绩

在疫情期间的创新



这一小节给大家比较系统性地介绍了 Microsoft Teams 产生的背景，和Office 365现有产品之间的关系，以及一路发展的主要历程。接下来就来谈一谈从平台的角度来说，它是怎么设想和定位的。

