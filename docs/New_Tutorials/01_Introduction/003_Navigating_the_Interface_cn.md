# 界面导航

该编辑器划分为八个独立的模块 (Modules)，每个模块都为游戏构建流程 (game-building process) 提供了不同的视图。这种划分有助于用户分离并理解开发流程 (development process) 中的各个环节。然而，由于可用的视图数量众多，理解如何在通用环境 (general environment) 以及各个独立的模块 (Module) 中进行导航的基本规则，可能需要一些时间。

下文将简要介绍在整个编辑器范围内通用的工具栏 (toolbars)、视图 (views) 和实用工具 (utilities)。

如果您希望了解每个模块 (Module) 的专属界面，可以参阅那些对相应模块进行更深入探讨的文章。

## 工具栏 (Toolbars)

在任何模块 (Module) 的顶部，您都会看到一组标签页 (tabs) 与工具栏 (toolbars)，它们将贯穿于编辑器的每一个视图 (view) 中。这些组件 (components) 会根据您所处的编辑器视图而略有变化，从而为每个模块 (Module) 提供相关的选项 (options)。

其主要组件自上而下依次是：**标题栏 (Title Bar)**、**文件栏 (File Bar)** 和 **主工具栏 (Main Toolbar)**。

![The Toolbar and Tab Collection](./resources/003_Navigating_the_Interface01.png)

**主工具栏 (Main Toolbar)** 是贯穿整个编辑器的常驻组件。尽管其外观像一个单一、完整的条状栏，但实际上它由三个组件 (components) 构成。

其中两个组件——最左侧的 **实用工具栏 (Utility Bar)** 和最右侧的 **导航栏 (Navigation Bar)**——是恒定不变的，无论您位于编辑器的哪个位置，其按钮都会保持一致。

工具栏的中央部分则是一个会针对当前模块 (Module) 而变化的动态区域。这部分可能包含：**地形栏 (Terrain Bar)**、**触发器栏 (Trigger Bar)**、**数据栏 (Data Bar)**、**AI栏 (AI Bar)**、**UI栏 (UI Bar)** 或 **过场动画栏 (Cutscene Bar)**。**导入器 (Importer)** 和 **文本编辑器 (Text Editor)** 没有专属的工具栏，但您会在 **总览管理器 (Overview Manager)** 中找到一个 **总览栏 (Overview Bar)**。

主工具栏如下图所示。

![Main Toolbar](./resources/003_Navigating_the_Interface02.png)

## 实用工具栏 (Utility Bar)

**实用工具栏 (Utility Bar)** 提供了数个适用于所有模块 (Module) 的标准功能 (functions)。您可以通过其绿色的按钮来识别此工具栏。

下方是该工具栏的图片及其功能解析。

![Utility Bar](./resources/003_Navigating_the_Interface03.png)

| 按钮          | 功能                                                         |
| ------------- | ------------------------------------------------------------ |
| 新建(Ctrl+N ) | 启动 **‘New Document’ (新建文档)** 窗口，允许您创建新的地图和 mods (模组)。 |
| 打开 (Ctrl+O) | 启动 **‘Open Document’ (打开文档)** 窗口，允许您打开本地文件或从 Battle.net 下载的文件。 |
| 保存 (Ctrl+S) | 保存当前文件。                                               |
| 撤销 (Ctrl+Z) | 还原在当前模块 (Module) 中所做的上一步更改。                 |
| 重做 (Ctrl+Y) | 重新应用上一个被 **‘撤销 (Undo)’** 所还原的更改。            |
| 剪切 (Ctrl+X) | 移除当前选中的内容，并将其保存至剪贴板 (clipboard)。         |
| 复制 (Ctrl+C) | 将当前选中的内容复制到剪贴板 (clipboard)。                   |
| 粘贴(Ctrl+V)  | 放置当前存储在剪贴板 (clipboard) 中的元素 (elements)。<br/>对于 **‘剪切 (Cut)’** 操作，此举也会清空剪贴板。对于 **‘复制 (Copy)’** 操作，剪贴板则会保留其内容。 |

请注意，这些操作是与上下文相关的 (context sensitive)：它们可以作用于何种类型的 元素 (elements)，完全取决于您当前在编辑器中所处的模块 (Module)。

这意味着，如果您位于 **触发器编辑器 (Trigger Editor)** 中，复制和粘贴操作将作用于诸如 Trigger、Action 或 Event 这样的元素。与此类似，如果您身处 **地形编辑器 (Terrain Editor)**，您则可以复制和粘贴完全不同的元素，例如 unit (单位) 或 doodad (装饰物)。

## 导航栏

**导航栏 (Navigation Bar)** 用于在各个模块 (Module) 之间进行切换。您可以通过其蓝色的按钮来识别此工具栏。

![Navigation Bar](./resources/003_Navigating_the_Interface04.png)

| Function              | Effect                                                   |
| --------------------- | -------------------------------------------------------- |
| 地形编辑器 (F5)       | 导航到地形编辑器。                                       |
| 触发编辑器 (F6)       | 导航到触发编辑器。                                       |
| 数据编辑器 (F7)       | 导航到数据编辑器。                                       |
| 文本编辑器 (F8)       | 导航到文本编辑器。                                       |
| 导入器(F9)            | 导航到导入器。                                           |
| AI编辑器 (Shift+F5)   | 导航到AI编辑器。                                         |
| UI编辑器 (Shift+F6)   | 导航到UI编辑器。                                         |
| 场景编辑器 (Shift+F7) | 导航到场景编辑器。                                       |
| 预览管理 (F12)        | 导航到预览管理界面。                                     |
| 测试文档 (Ctrl+F9)    | 启动当前地图来进行测试，正如在“首选项”一栏中描述的一样。 |

该工具栏承载了极为实用的 **‘测试文档 (Test Document)’** 功能，而您将会频繁地使用到它。

此外，您还可以通过它导航至 **总览管理器 (Overview Manager)**，其功能相当于一个对整个项目及各个模块进行审视的宏观视图 (bird's eye view)。

## 其他工具栏

**标题栏 (Title Bar)** 会显示您在编辑器中的当前位置，以及当前活动项目的位置和文件结构。如下方示例所示。

![Title Bar](./resources/003_Navigating_the_Interface05.png)

当从战网 (Battle.net) 访问文件时，文件结构将采用 [Battle.net: FileName] 的格式。

在 **文件栏 (File Bar)** 中，您同样可以找到许多与项目各个方面相关的标签页 (tabs) 及其选项 (options)。与 **主工具栏 (Main Toolbar)** 类似，无论您位于何处，它都会提供 **文件 (File)**、**编辑 (Edit)**、**视图 (View)**、**地图 (Map)**、**模块 (Modules)**、**窗口 (Window)** 和 **帮助 (Help)** 这些标签页。根据您在编辑器中的当前位置，您还会发现其他一些与上下文相关的 (context-sensitive) 选项。

![File Bar](./resources/003_Navigating_the_Interface06.png)

此外，编辑器还提供了一个与上下文相关的 (context-sensitive) 工具栏，其上的功能 (functions) 仅对您当前所在的位置可用且相关。我们将在那些描述编辑器主要区域——八个模块 (Modules) 和 **总览管理器 (Overview Manager)**——的文章中，对这些内容进行更详细的讨论。

## 快捷键 (Hotkeys)

该编辑器为快捷键 (hotkeys) 提供了广泛的支持，并允许对所有标准操控 (standard controls) 进行完全自定义。您可以为几乎任何可用的 function (功能) 设置快捷键，且其中大部分功能并未预设默认快捷键。

您可以通过导航至 文件 (File) ▶︎ 配置操控 (Configure Controls) 来访问快捷键的配置界面。此操作将启动 **‘Configure Controls’ (配置操控)** 窗口，如下图所示。

![Hotkey Configuration](./resources/003_Navigating_the_Interface07.png)

