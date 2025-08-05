---
title: Editor Introduction
author: jrepp
category: 01_Introduction
translation: lawbda
---
# 简介

星际争霸2编辑器是一整套用于星际争霸2游戏开发的工具组。这些工具与暴雪自己用于最新版本星际争霸开发时所用到的工具高度的一致。与战网和暴雪街机模式（Arcade）一起，编辑器提供了一个健壮的游戏开发平台、主持游戏系统以及多人模式网络。

![Editor Tool Suite](./resources/001_Editor_Introduction01.png)

星际争霸II编辑器 (StarCraft II Editor) 首次于2010年伴随《自由之翼》(Wings of Liberty) 正式发布，它为玩家提供了访问游戏内全部美术与 Assets (资源) 的权限。

这一举措延续了暴雪公司的一项悠久传统，即向其玩家社区完全开放自家的创作工具，该传统始于1994年《魔兽争霸II：黑暗之潮》(WarCraft II: Tides of Darkness) 的发布。

随着《星际争霸II》每一部资料片的推出，这款编辑器也获得了更多的内容增补，其中甚至包含了一个囊括了《魔兽争霸III》(Warcraft III) 全部 Assets 的官方资源包。

## 街机模式(Arcade)

对此，《星际争霸II》的模组社区 (modding community) 作出了积极响应，创作了数以千计的自定义地图与 mods (模组)。

所有这些作品都可以在一个由暴雪托管、名为 Arcade 的平台上找到，玩家可以通过《星际争霸II》游戏客户端 (game client) 访问该平台。

在 Arcade 中，玩家能够在一个充满活力的在线游戏开发社区 (online game development community) 内进行探索、游玩与分享。

使用该编辑器将为您开启通往这个社区的大门，您将能够展示自己的项目、将其呈现给大众、获取反馈、探索他人的游戏作品、从中获得灵感，以及最重要的——尽情游玩。

![Games in the Arcade](./resources/001_Editor_Introduction02.png)

## 银河编辑器的潜力

银河编辑器是一款具备专业品质的游戏引擎 (game engine)，拥有广泛的功能，其中包含了其自有的脚本语言 (scripting language)。即便如此，您在入门时并不需要具备编程经验。如果您希望开始学习如何使用该编辑器，那么本网站正是您所需要的起点。本网站旨在为所有学习使用《星际争霸II》编辑器的用户，提供一份核心手册与课程规划。因此，请继续阅读引言部分，然后开始探索本网站的内容。

由于其作为首批用于地图设计的社区工具之一的历史渊源，该编辑器常被称为“地图编辑器” (Map Editor)。然而，该编辑器的功能远不止于简单的地图创建。它是一款强大而稳健的游戏引擎 (game engine)，您可以使用它来构建各种不同类型的游戏、地图，以及对《星际争霸II》体验进行修改的模组。

![Some of the Varied Community Creations](./resources/001_Editor_Introduction03.png)

如果您是竞技《星际争霸II》的爱好者，您可以为其他玩家创建新的对战地图 (melee maps) 以供他们交战。您的地图甚至可能声名鹊起，成为某项顶级电子竞技锦标赛中决胜局的比赛场景。

在此基础上，您可以开始微调并探索《星际争霸》的游戏玩法 (gameplay)。您可以对任何现有的《星际争霸II》对战地图应用自定义数据 (data) 修改，这也包括您自己创建的地图。随后，您可以将这些地图构建为完整的自定义战役 (custom campaigns)，在星际争霸的世界中讲述您自己的故事。

除此之外，您也可以着手创建属于您自己的游戏类型 (game type)。开发者们已经创作出了从简单的环境场景，到复杂的塔防 (Tower Defense) 地图，乃至宏大的RPG史诗等各式各样的作品。您可以从《魔兽争霸》与《星际争霸》悠久的自定义游戏历史中汲取灵感——这是一个充满活力的模组文化 (modding culture)，它催生了诸如塔防 (Tower Defense) 和英雄乱斗 (Hero Brawlers) 等游戏类型，例如 DotA 以及我们自家的《风暴英雄》(Heroes of the Storm)（一款其原型 (prototypes) 正是构建于《星际争霸II》编辑器之上的游戏）。

编辑器中的模块
-----------

模块 (Modules) 是主编辑器的主要功能分区。每一个模块都呈现为一个更小型、更专注的编辑器，服务于游戏开发流程 (game development process) 中的特定环节。作为独立的工具，每一个模块 (Module) 都高度特化；而作为一个整体，它们赋予您构建一款完整游戏所需的创作控制权。

- **地形编辑器 (Terrain Editor):** 地形编辑器允许您塑造地形，创建游戏世界。对战地图 (Melee map) 的作者可以用它来绘制用于竞技对战的地貌；而对于其他类型的创作，这便是构建世界外观的主要工具。
- **触发器编辑器 (Trigger Editor):** 触发器编辑器 (Trigger Editor) 是您为游戏注入生命与逻辑 (logic) 的地方。您可以选择使用《星际争霸II》的内置脚本语言 (scripting language)，或是使用一套对编程新手十分友好的图形用户界面 (GUI) 系统。
- **数据编辑器 (Data Editor):** 数据编辑器 (Data Editor) 是存放已有游戏 Assets 和您独有创作的库房。在这里，您可以构筑诸如单位 (units)、增益效果 (buffs)、技能 (abilities)、效果 (effects)、声音 (sounds) 等等内容。随着您游戏创作经验的增长，这些创作物将始终存在，并随时可以在新的游戏场景 (playfields) 中被复用。
- **导入器 (Importer):** 导入器 (Importer) 允许您从编辑器外部引入自定义设计的 Assets，包括 3D 模型 (3D models)、图像 (images)、音乐 (music) 或任何您需要的其他内容。
- **UI编辑器 (UI Editor):** UI编辑器 (UI Editor) 为您提供了定义和创建自定义界面 (custom interfaces) 的工具，或是修改《星际争霸II》中已有界面的工具。
- **过场动画编辑器 (Cutscene Editor):** 过场动画编辑器 (Cutscene Editor) 允许您创建自己的电影式镜头 (cinematics)，它既可以作为游戏内叙事 (in-game storytelling) 的工具，也可用于创作在游戏外呈现的机械电影 (Machinima) 内容。
- **文本编辑器 (Text Editor):** 文本编辑器 (Text Editor) 允许您更改游戏中各类文本的字体 (fonts)、样式 (styles) 和其他排版效果 (typographical effects)。
- **AI编辑器 (AI Editor):** AI编辑器 (AI Editor) 是您创建和修改人工智能 (artificial intelligence) 的地方。这些AI决定了单位的行为 (unit actions)，可用于打造终极的竞技对手，或是定义您自定义游戏中由电脑控制的角色的思维模式。

## 踏上征程！

现在，正是您开启学习与创作之旅的绝佳时机。在您投身于《星际争霸II》编辑器所蕴含的无限创作可能之际，本网站将成为您的向导。

请继续探索，并尽享其乐。

![Image](./resources/001_Editor_Introduction04.png)

冒险在等待！ (图源: njordys)
