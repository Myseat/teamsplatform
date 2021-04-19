---
description: 微软历史上成长速度最快的应用
---

# Microsoft Teams 及其发展

## Microsoft Teams 诞生的背景和战略意义

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

## Microsoft Teams 和Office 365其他产品的关系

即便是如此，从Microsoft Teams 面世第一天开始，也伴随着各种疑问，其中被客户问的最多的问题就是：Office 365已经有Outlook，Skype for Business等全系列产品可以做沟通与协作，那么Teams 的具体定位是什么呢？

![](../.gitbook/assets/image%20%2815%29.png)

Microsoft Teams为团队而生，它天生具备的功能就包括了聊天，音视频会议，以及共享文件和协作。作为一个现代版的工具，它也具备一定社交化的功能。这些功能和原先的Outlook，Skype for Business, SharePoint 和OneDrive，以及Yammer都有重叠。但是Teams 并不是重新开发这些功能，而是直接将他们整合进来，用户可以仅仅通过一个应用，即可以完成全方位的沟通和协作，除了收发邮件。

下面这一张图进一步解释了这种关系

![](../.gitbook/assets/image%20%2817%29.png)

> 以上这张截图来自于官方文档 [https://techcommunity.microsoft.com/t5/microsoft-teams/new-teams-it-architecture-posters-published/m-p/480928](https://techcommunity.microsoft.com/t5/microsoft-teams/new-teams-it-architecture-posters-published/m-p/480928)，仅提供英文版本。链接网页中还有其他一些很有参考价值的架构图。

为什么Microsoft Teams不把邮件的功能也整合进来呢？ 这是由于邮件这种沟通方式，和Microsoft Teams所主张的（也是业界目前推崇的）“基于对话的沟通”是两种不同的方式。邮件并没有过时，它仍然适合于很多正式的、私密性的沟通，包括内部和外部。但很多时候用邮件就会显得很臃肿并且麻烦，例如在团队讨论一个活动的安排，来来回回几十个邮件，沟通效率极低，甚至让人厌烦，你会觉得这种方式真的像远古时代的恐龙那样笨重。市场总是需要一些新的东西，主要是社会发展的需要（人类的沟通协作方式在发生肉眼可见的变化），另外一小部分是由于商业的需要。

不去重复做已经有的东西，快速地把核心的框架和平台搭建起来，并且投放到市场去接受检验，并且快速地进行迭代开发，这就是Microsoft Teams 能成为微软历史上成长速度最快的应用的原因。下面简单回顾一下它面世以来的主要几个里程碑吧。

> 关于Microsoft Teams 成为微软历史上成长速度最快的应用的说法，请参考官方文档 [https://pulse.microsoft.com/en/work-productivity-en/na/fa2-reasons-why-you-should-start-using-microsoft-teams-today/](https://pulse.microsoft.com/en/work-productivity-en/na/fa2-reasons-why-you-should-start-using-microsoft-teams-today/) 的第一段。

## Teams 主要里程碑和路线图

1. **2017年3月14日，Microsoft Teams 正式对全球客户可用。**当时的官方发布会邀请，你可以通过这里找到。[https://www.microsoft.com/en-us/microsoft-365/blog/2017/03/07/join-us-for-an-online-event-to-celebrate-the-global-availability-of-microsoft-teams/](https://www.microsoft.com/en-us/microsoft-365/blog/2017/03/07/join-us-for-an-online-event-to-celebrate-the-global-availability-of-microsoft-teams/)
2. **2018年3月12日，微软发布Microsoft Teams一周年成绩单**：在这一年中，Teams 在新功能和客户使用量方面都取得了显着提升。现在，181 个市场的 20 万个组织和 39 种语言在使用 Teams，包括 A.P. Moller–Maersk、ConocoPhillips、通用汽车、梅西百货、NASCAR、Navistar、RLH Corporation 和 Technicolor。详情请参考 [https://www.microsoft.com/zh-cn/microsoft-365/blog/2018/03/12/microsoft-teams-turns-1-advances-vision-for-intelligent-communications/](https://www.microsoft.com/zh-cn/microsoft-365/blog/2018/03/12/microsoft-teams-turns-1-advances-vision-for-intelligent-communications/) 
3. **2018年7月12日，微软发布免费版本的Microsoft Teams**。详情请参考 [https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-a-free-version-of-microsoft-teams/ba-p/214592](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-a-free-version-of-microsoft-teams/ba-p/214592)。



你可以随时通过 [https://www.microsoft.com/zh-cn/microsoft-365/roadmap?filters=Microsoft%20Teams](https://www.microsoft.com/zh-cn/microsoft-365/roadmap?filters=Microsoft%20Teams) 了解到Microsoft Teams的路线图。你也可以把这个地址 [https://www.microsoft.com/zh-cn/microsoft-365/RoadmapFeatureRSS/](https://www.microsoft.com/zh-cn/microsoft-365/RoadmapFeatureRSS/) 加入到RSS阅读器（例如Outlook），以便随时收到最新的功能通知。

![](../.gitbook/assets/image%20%2816%29.png)

> 截图于 2021-4-19日

## 疫情期间的创新





这一小节给大家比较系统性地介绍了 Microsoft Teams 产生的背景，和Office 365现有产品之间的关系，以及一路发展的主要历程。接下来就来谈一谈从平台的角度来说，它是怎么设想和定位的。

