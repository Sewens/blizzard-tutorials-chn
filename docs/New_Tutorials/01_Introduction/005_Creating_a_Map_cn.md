# 创建一个地图

任何项目的第一步，都是创建一个新的文档，即一张 **地图 (map)** 或是一个 **模组 (mod)**。

在创建文档时，您将会看到一些 **选项 (options)**，用以帮助您快速配置您的项目。所有这些初始 **配置 (configurations)**，稍后都可以在 **编辑器 (Editor)** 本身中进行更改。

## 创建地图选项

当编辑器启动时，您可以从任何编辑器界面的最左上角导航到文件选项卡中。

[![File Menu](./resources/005_Creating_a_Map01.png)](./resources/005_Creating_a_Map01.png)
*文件菜单*

这将指引你来到**“新文档”**窗口，在此处你可以选择创建何种类型的文档。

[![Choosing Document Type](./resources/005_Creating_a_Map02.png)](./resources/005_Creating_a_Map02.png)
*选择文档类型*

在这个场景中，通过点击左侧的按钮选择**Arcade地图**，之后点击下一步来确认。

之后将进入依赖部分的配置，如下图所示。

[![Choosing Dependency](./resources/005_Creating_a_Map03.png)](./resources/005_Creating_a_Map03.png)
*选择依赖项*

**依赖项 (Dependencies)** 描述了哪些 **mod** 文件将为项目提供 **Assets**。

您始终可以通过导航至 **‘Custom’ (自定义)** 选项卡，然后不作任何选择来继续操作。这样便会创建一个不含任何 **mod** 文件依赖项的、完全空白的项目。

在此示例中，您将使用庞大的星际争霸**Assets** 库，它通常被称为 **‘标准依赖项 (standard dependencies)’**。能够访问这些标准依赖项，是使用该编辑器进行创作的主要优势之一。

若要导入《星际争霸》**Assets** 的最新版本数据，请选择 **‘虫群之心 (Heart of the Swarm)’** 标准依赖项，然后选择 **‘Next’ (下一步)** 以继续。此操作将使您进入地图配置环节，如下图所示。

## 地图配置

[![Example Generation Options](./resources/005_Creating_a_Map04.png)](./resources/005_Creating_a_Map04.png)
*生成选项的示例*

**地图配置 (map configuration)** 界面是您进行地形初始外观基本设定的地方。各个选项的效果将在下表中逐一解析。

| 属性                                 | 效果                                                         |
| ------------------------------------ | ------------------------------------------------------------ |
| **尺寸 (Dimensions)** (宽度 x 高度)  | 设定地图的初始完整尺寸。您可以稍后通过 地图边界 (Map Bounds) 选项进行更改。尺寸范围为32至256个单位，以8为增量。 |
| **可游戏尺寸 (Playable Size)**       | 地图中单位可以寻路 (path) 的实际区域，该区域是基于地图每侧一个硬编码 (hard-coded) 的可变缓冲区 (variable buffer) 进行校正的。在某些极小的尺寸下，此缓冲区会被忽略。 |
| **尺寸描述 (Size Description)**      | 对地图尺寸的基本描述。选项包括：**微小 (Tiny)**、**小型 (Small)**、**中型 (Medium)**、**巨型 (Huge)** 和 **史诗 (Epic)**。 |
| **使用地形 (Use Terrain)**           | 取消勾选此项会中止地形的生成。尽管在某些情况下您可能需要一个无地形的地图，但其在功能上类似于一个 mod。 |
| **纹理集 (Texture Set)**             | 选择地图的 ‘地形类型 (Terrain Type)’，即用于构建您环境中地面的八种纹理的调色板 (palette)。这同样适用于菌毯视觉效果 (creep visuals)、悬崖类型 (cliff types)、光照 (lighting) 和环境音效集 (atmospheric sound sets)。 |
| **初始纹理 (Initial Texture)**       | 生成时，整个地形将被绘制为此纹理集中的这一种单一类型。       |
| **基础高度 (Base Height)**           | 所有地形都将在此默认高度上生成。如果 **‘添加随机高度 (Add Random Height)’** 选项未被勾选，地形将生成为平滑的表面。 |
| **添加随机高度 (Add Random Height)** | 在 **基础高度 (Base Height)** 中创建随机的起伏，其幅度由 **‘强度 (Strength)’** 和 **‘变化度 (Variability)’** 选项的滑块决定。这对于生成更具自然感的地形基础很有帮助。 |

遵循我们上方 **‘示例生成指引 (Example Generation Guidelines)’** 图片中设定的指引，您应该会得到一个如下图所示的地图。这张地图已为开始一个新项目做好了准备。此时，保存您的文件是明智之举。

[![Newly Generated Char Rock](./resources/005_Creating_a_Map05.png)](./resources/005_Creating_a_Map05.png)
*新生成的红石地貌*
