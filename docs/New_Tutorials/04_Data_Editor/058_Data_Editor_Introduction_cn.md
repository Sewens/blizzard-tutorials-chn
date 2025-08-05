# 数据编辑器介绍

**数据编辑器 (Data Editor)** 容纳了编辑器中所有的数据Assets。一个项目的每一片data都是使用此处所见的基础类型构建而成。它是一个既深度又强大的系统，为用户提供了极大的控制权——其程度是暴雪编辑套件中前所未有的。

[![Data Editor in Use](./resources/058_Data_Editor_Introduction1.png)](./resources/058_Data_Editor_Introduction1.png)
*使用中的数据编辑器*

在 **数据编辑器 (Data Editor)** 内部，您会发现一套强大的功能集 (feature set) 来支持其编辑功能。您应当注意，data 会在您工作时动态更新，使得变更能够快速地 **传播 (propagate)** 至整个项目。此处也有多个可视化选项，可用于概览任何 data 构筑体。这些对于建立起对引擎运作方式的直观感知 (tactile sense) 非常有帮助。或许最重要的一点是，所有星际争霸的Assets均可在此获取，并能通过 **数据编辑器 (Data Editor)** 查看。您可以在此仔细地检视它们并从中学习，或是 **重新调整其用途 (repurpose)** 以用于您自己的 mods。

## 数据目录

编辑器中的数据被组织成**目录 (Catalogs)**，每一个目录都包含当前项目中一个特定数据类型的所有 **实例 (instance)** 的列表。您必须导航至一个特定数据类型的目录，才能创建或管理该特定类型的任何数据。每个目录都提供了一个视图，可查看其关联类型的所有数据字段 (data fields)，以及一些与上下文相符的选项。**数据编辑器 (Data Editor)** 中总计有87个目录，不过大多数用户会发现他们的工作将集中于其中的一小部分。这87个目录中的大部分是由高度特化的数据类型组成的，其中许多您将极少使用。

目录的一些示例包括大家所熟悉的 **技能 (Abilities)** 和 **单位 (Units)** 这类游戏类型，以及像 **模型 (Models)** 和 **声音 (Sound)** 这类美术 Assets。上文提到的一些更特定的类型则包括 **物理材质 (Physics Materials)**、**光标 (Cursors)** 和 **成就 (Achievements)**。在本段下方您会找到引擎目录的完整列表。值得注意的是，这些目录被组织成宽泛的类别，例如 **游戏数据 (Game Data)** 或 **演算体数据 (Actor Data)**，以反映不同数据类型的不同用途。

**游戏数据[13]**

  - 技能 (Abilities) --- 行为 (Behaviors) --- 效果 (Effects)
- 足印(Footprints) --- 物品 (Items) --- 拾取物 (Loot)
- 移动器 (Movers) --- 要求 (Requirements) --- 炮台 (Turrets)
- 单位 (Units) --- 升级 (Upgrades) --- 验证器 (Validators)
- 武器 (Weapons)

**战役数据[13]**

  - 部队类别 (Army Categories) --- 部队单位 (Army Units) --- 部队升级 (Army Upgrades)
- Bank条件 (Bank Conditions) --- 战役 (Campaigns) --- 角色 (Characters)
- 指挥官 (Commanders) --- 对话(Conversations) --- 对话状态 (Conversation States)
- 位置 (Locations) --- 地图 (Maps) --- 目标 (Objectives)
- 预载 (Preload)

**演算体数据[3]**

- 演算体 (Actors) --- 附加方式 (Attach Methods) --- 光束 (Beams)

**美术和声音资源[12]**

- 按钮 (Buttons) --- 数字音效 (Digital Sound Effects) --- 镜头光晕集 (Lens Flare Sets)
- 光源 (Lights) --- 模型 (Models) --- 混响效果 (Reverb Effects)
- 形状 (Shapes) --- 声音 (Sounds) --- 声音独占性 (Sound Exclusivities)
- 混音快照 (Sound Mix Snapshots) --- 音轨 (Soundtracks) --- 纹理 (Textures)

**地形数据[9]**

- 地形悬崖 (Terrain Cliffs) --- 地形悬崖网格 (Terrain Cliff Meshes) --- 战争迷雾数据 (Fog of War Data)
- 物理材质 (Physics Materials) --- 地形类型 (Terrain Types) --- 地形物体 (Terrain Objects)
- 地形纹理 (Terrain Textures) --- 地形道路 (Terrain Roads) --- 水体 (Water)

**英雄数据[11]**

- 神器 (Artifacts) --- 神器栏位 (Artifact Slots) --- 配置 (Configs)
- 英雄 (Heroes) --- 英雄技能 (Hero Abilities) --- 英雄统计 (Hero Statistics)
- 坐骑 (Mounts) --- 皮肤 (Skins) --- 天赋 (Talents)
- 天赋档案 (Talent Profiles) --- 配音 (Voice Overs)

**界面数据[6]**

- 警报 (Alerts) --- 捆绑包 (Bundles) --- 镜头 (Cameras)
- 光标 (Cursors) --- 游戏UI数据 (Game UI Data) --- 信号 (Pings)

**高级数据[20]**

- 成就 (Achievements) --- 成就条款 (Achievement Terms) --- 强化 (Boosts)
- 游戏玩法数据 (Gameplay Data) --- 兽群 (Herds) --- 兽群节点 (Herd Nodes)
- 物品类别 (Item Classes) --- 物品容器 (Item Containers) --- 动力学 (Kinetics)
- 种族 (Races) --- 要求节点 (Requirement Nodes) --- 奖励 (Rewards)
- 得分结果 (Score Results) --- 得分值 (Score Values) --- 战术AI冷却 (Tactical AI Cooldowns)
- 战术AI数据 (Tactical AI Data) --- 目标搜寻 (Target Finds) --- 目标排序 (Target Sorts)
- 奖杯 (Trophies) --- 用户类型 (User Types)

## 数据编辑器界面

[![Data Editor Interface View](./resources/058_Data_Editor_Introduction2.png)](./resources/058_Data_Editor_Introduction2.png)
*数据编辑器界面*

您可以使用如下图所示的 **目录选项卡 (Catalog Tabs)** 来导航 **数据编辑器 (Data Editor)** 的各个目录。

[![Catalog Tabs](./resources/058_Data_Editor_Introduction3.png)](./resources/058_Data_Editor_Introduction3.png)
*数据分类选项*

每个目录都有一个关联的选项卡，用于访问其 data 列表。您可以使用绿色的、加号形状的 **目录开启器 (Catalog Opener)** 将一个选项卡带入项目中。一旦您选择了一个选项卡，它便会在 **对象列表 (Object List)** 中填充该目录的 data，如下图所示。

[![Object List](./resources/058_Data_Editor_Introduction4.png)](./resources/058_Data_Editor_Introduction4.png)
*对象列表*

该列表根据多个与上下文相关的属性，例如 **来源 (Source)**、**ID编号 (#)**、**对象家族 (Object Family)** 和 **种族 (Race)**，来组织整个数据目录。正如下图所示，对于选中的实例，其 data 结构的完整层级将在 **对象浏览器 (Object Explorer)** 中显示。

[![Object Explorer](./resources/058_Data_Editor_Introduction5.png)](./resources/058_Data_Editor_Introduction5.png)
*对象浏览器*

对于像 **单位 (Units)** 这样更高层级的构筑体，此浏览器为检视一个数据的所有内容提供了一个至关重要的、自顶向下的视图。**对象浏览器 (Object Explorer)** 或 **对象列表 (Object List)** 中的任何数据，都会在 **字段列表 (Fields Listing)** 中显示其数据字段，如下图所示。

[![Fields Listing](./resources/058_Data_Editor_Introduction6.png)](./resources/058_Data_Editor_Introduction6.png)
*字段列表*

**字段列表 (Fields Listing)** 是 **数据编辑器 (Data Editor)** 的数据录入区。在这里，data 可以通过用户输入被直接修改。由于可供编辑的目录和字段类型繁多，此处提供了一系列视图选项，以使该列表尽可能易于访问。您可以在 **数据栏 (Data Bar)** 中找到它们。

[![Data Bar](./resources/058_Data_Editor_Introduction7.png)](./resources/058_Data_Editor_Introduction7.png)
*数据栏*

下方是各种视图选项的解析。

| 操作                       | 效果                                                         |
| -------------------------- | ------------------------------------------------------------ |
| **查看原始数据**           | 将所有 data 从其更易于使用的 **名称值 (Name values)** 更改为其在后端代码中使用的 **原始ID值 (raw ID values)**。 |
| **以树状结构显示对象列表** | 将 **对象列表 (Object List)** 显示为一组结构化的文件夹。     |
| **显示所有对象来源**       | 将原始的、未修改的源 data 与该 data 的任何当前版本并列显示。 |
| **显示对象浏览器**         | 切换 **对象浏览器 (Object Explorer)** 的可用性。             |
| **在数据导航器中查看**     | 在 **数据导航器 (Data Navigator)** 中将当前选中的 data 实例可视化。 |
| **表格视图**               | 将 **字段列表 (Fields Listing)** 显示为其所有独立字段的列表形式。 |
| **细节视图**               | 将 **字段列表 (Fields Listing)** 显示为其录入窗口或子编辑器的组合。 |
| **XML视图**                | 将 **字段列表 (Fields Listing)** 显示为其原始的 XML 文件。   |
| **按来源排序字段**         | 根据每个字段的 data 来源来组织列表。                         |
| **显示基础字段标签**       | 在任何源自“基础”来源的 data 字段上显示“(基础)”标签。         |
| **显示字段类别**           | 显示每一片 data 的任何类别标题。                             |
| **合并结构值**             | 将任何相关的字段合并为一个单一字段。                         |
| **显示字段差异**           | 显示 data 字段中的任何差异。                                 |
| **XML语法高亮 **           | 为XML视图启用基于类型的彩色高亮。                            |
| **提交XML变更**            | 保存对 XML 文件所做的任何当前未保存的更改。                  |

这些选项包括结构化的 **字段列表 (Fields Listing)** 视图：**表格视图 (Table View)**、**细节视图 (Detail View)** 和 **XML视图 (XML View)**，如下图所示。

[![Table View - Detail View -- XML View](./resources/058_Data_Editor_Introduction8.png)](./resources/058_Data_Editor_Introduction8.png)
*表格视图 - 细节视图 -- XML视图*

这些视图选项也可以从 **数据编辑器 (Data Editor)** 的 **视图 (View)** 选项卡访问。

![View Tab](./resources/058_Data_Editor_Introduction9.png)
*视图选项卡*

在每个图层中都有不同的选项可用。您可以从主地形视图最左侧的大面板访问它们。这被称为 **UI面板 (UI Panel)**。

**UI面板 (UI Panel)** 会根据您当前的图层而变化；每个图层都有一个 **调色板 (Palette)**，提供了该图层的大部分主要控件。这些调色板是专为在当前图层中使用而设计的。

您也应注意到顶部的 **文件 (File)** 选项卡提供了许多选项。这些选项被细分为多个子选项卡，将在以下各节中进行描述。

## 子编辑器

在某些情况下，您会发现在字段编辑期间，会有更特化的、嵌套的编辑器可用。这些 **子编辑器 (Subeditors)** 包括 **演算体事件编辑器 (Actor Events Editor)**、**足印编辑器 (Footprints Editor)** 和 **声音编辑器 (Sound Editor)**。它们如下图所示。

![](./resources/058_Data_Editor_Introduction10.png)
*演算体事件编辑器--脚印编辑器--声音编辑器*

## 数据可视化

随着您项目中的 data 结构不断增长并交织在一起，拥有一些可视化选项会很有用，这样您就可以更好地了解您的项目正在做什么。**数据编辑器(Data Editor)** 为此提供了几个选项，其中最著名的是如下图所示的**数据导航器 (Data Navigator)**。

[![Data Navigator](./resources/058_Data_Editor_Introduction11.png)](./resources/058_Data_Editor_Introduction11.png)
*数据导航器*

该导航器绘制出每片 data 之间的链接，以一种可读的方式呈现整个实例的 **数据层级结构 (data hierarchy)**。另一个有用的配置是可用于 **对象浏览器 (Object Explorer)** 的 **显示解释链接 (Show Explain Link)** 选项。这会将数据连接的一个简化版本显示至一个 **输出面板 (output panel)**，如下图所示。

![Show Explain Link](./resources/058_Data_Editor_Introduction12.png)
