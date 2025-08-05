# 创建模组

尽管地图文件始终是编辑器的最终产物，但 mod 文件才是任何项目真正的核心所在。通过将 data 从构建好的地图中分离出来，mods 使得项目能够被更自由地开发与分享。这种关系的好处并不仅限于易用性。Mods 将项目的可能性扩展到了任何暴雪编辑器都前所未及的程度。而探索这一点的最佳方式，便是亲身试验编辑器构建、组合及运用 mods 的能力。

## 构建一个基础模组

通过导航至 文件 (File) ▶︎ 新建 (New) 来创建一个新文档。此操作将启动 **‘New Document’ (新建文档)** 窗口，您应在其中选择创建 **‘依赖型模组 (Dependent Mod)’**。点击 **‘Next’ (下一步)** 进入 **‘选择依赖项 (Choose Dependencies)’** 选项卡，选择 **‘Custom’ (自定义)**，然后点击 **‘OK’ (确定)**。现在，使用 **地形模块 (Terrain Module)** 导航至 模组 (Mod) ▶︎ 模组信息 (Mod Info)，启动 **‘Mod Properties Window’ (模组属性窗口)**。在该窗口的 **‘Name’ (名称)** 字段中输入标题“Tutorial Dependency”。您也可以在描述字段中输入“This is a tutorial dependency.”。请参考下图作为指引。

[![Mod Creation & Configuration Order](./resources/007_Creating_Mods01.png)](./resources/007_Creating_Mods01.png)
**模组创建与配置流程**

您现在已经创建了一个简单的 mod。**‘依赖型模组 (Dependent Mod)’** 是基础的 mod 类型。其名称源于这样一个事实：任何被置入 mod 的地图，都会进入一种被称为 **依赖项 (Dependency)** 的关系中。当您在 **‘选择依赖项 (Choose Dependencies)’** 视图下选择了 **‘Custom’ (自定义)** 并将其留空时，该 mod 文件便被设定为不含任何基础依赖项。一个空的 mod 是一个完全自定义项目的最佳起点。您的 mod 中唯一的信息，便是您在上一步中填入的少量细节。

将您的 mod 以“Tutorial Dependency”为名，保存到您偏好的位置。《星际争霸》会为 mods 分配 .SC2Mod 的文件扩展名。

## 为模组添加数据

一个 mod 的最终目的是成为 Assets 的容器。您可以通过为您的基础 mod 填充一些触发器来进一步了解这一点。请注意，一个mod文件需要一个**触发库 (trigger library)** 来存放其触发器。而地图文件则不然，它可以支持位于库之外的触发器。

移动至 **Trigger 模块**，您将在这里创建一个 **Trigger 库 (Trigger Library)**。您可以通过右键点击 **Triggers 面板** 并导航至 库 (Library) ▶︎ 新建库 (New Library) 来完成此操作。新的库将会出现在 **列表面板 (List Panel)** 中。将其重命名为 “Tutorial Library”。

现在，再次选中 **Trigger 面板**，通过导航至 新建 (New) ▶︎ 新建动作定义 (New Action Definition) 来添加一个 **action 定义**。将此定义重命名为“Dependency Message”。在此 action 定义中，通过 动作 (Actions) ▶︎ 调试信息 (Debug Message) 来添加一个新的动作。

最后，将此动作的文本字段更改为“This is a message from the dependency.”。您最终应该会得到一个如下图所示的成果。

[![Mod's Trigger Library](./resources/007_Creating_Mods02.png)](./resources/007_Creating_Mods02.png)
**模组的触发库**

## 使用一个模组作为依赖项

既然您已经配置好了您的 mod 文件，您需要创建一个新的地图文件来将其作为 **依赖项 (dependency)** 进行测试。您可以通过导航至 文件 (File) ▶︎ 新建 (New) ▶︎ Arcade 地图 (Arcade Map) 来完成。在地形界面点击 **‘重置为默认值 (Reset to Defaults)’**，并将此地图保存为“Tutorial Mod Test”。

要将一个mod作为依赖项添加到此地图，请导航至 文件 (File) ▶︎ 依赖项 (Dependencies)。根据默认的地图配置，**‘Liberty (Mod)’** 这个标准依赖项已被包含在内。由于您想要添加一个自定义 mod，请选择 **‘添加其他 (Add Other)’**。

[![Dependency Adding View](./resources/007_Creating_Mods03.png)](./resources/007_Creating_Mods03.png)
**添加依赖项视图**

此操作将启动一个 **‘选择文档 (Choose Document)’** 窗口，它允许您访问存储在本地和战网 (Battle.net) 上的 mod 文件。在此例中，您已经将所需的 mod 文件保存在本地。

使用提供的文件浏览器找到它并点击 **‘OK’ (确定)**，之后您将被带回到依赖项选择界面。

[![Custom Dependency Added](./resources/007_Creating_Mods04.png)](./resources/007_Creating_Mods04.png)
*自定义添加的依赖*

点击 **‘OK’ (确定)** 以完成依赖项的添加，然后重新打开 **Trigger 模块**。现在是确保您启用了库视图的好时机，您可以通过 视图 (View) ▶︎ 显示库 (Show Libraries) 来开启它。您自定义 mod 中的触发数据现在应该已变为可见并可供使用。在顶部的 **列表面板 (List Panel)** 中，您将看到名为 **Built-In**、**Liberty** 和 **Tutorial Library** 的触发库。

![Imported Library from Mod](./resources/007_Creating_Mods05.png)
*从Mod中导入的库*

通过将一个 **‘Dependency Message’** 行为添加到地图的 Melee Initialization trigger 中，来测试该依赖项的功能性。在 **‘Actions’** 标题下右键点击，然后导航至 新建 (New) ▶︎ 新建动作 (New Action) ▶︎ Dependency Message。

请注意，导入的动作定义会将其来源显示为 **‘Tutorial Library’**，而非暴雪官方的 **‘Built-in’** 或 **‘Liberty’** 库。在此之后，删除所有无关的默认对战动作。这样您将得到如下的配置。

[![Dependency Action Definition in Use](./resources/007_Creating_Mods06.png)](./resources/007_Creating_Mods06.png)
**使用中的依赖项动作定义**

现在以测试模式运行您的文档，应该会得到一个与下图类似的结果。

[![Output from Dependency Library](./resources/007_Creating_Mods07.png)](./resources/007_Creating_Mods07.png)*来自依赖项库的输出*
