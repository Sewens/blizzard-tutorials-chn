好的，收到。作为一名在即时战略（RTS）和暴雪游戏圈子里摸爬滚打了多年的老兵，同时又对引擎和编辑器技术充满热情，我非常理解你的需求。一份糟糕的教程翻译会毁掉一个创作者的入门体验，而一份精准、专业的翻译则能为一个社区注入新的活力。

这不仅仅是语言的转换，更是知识和操作逻辑的精准传递。以下是我为你设计的，用于游戏编辑器教程翻译的提示词系统（Prompt System）。该系统包含一个核心提示词模板和一套详细的执行准则。

---

### **核心提示词系统 (Core Prompt System)**

你可以在每次翻译任务开始时，将以下模板作为基础指令提供给AI。

**Master Prompt Template:**

```
# Role and Goal
You are a professional technical translator with deep expertise in game development, specifically focusing on game engines, editors (like StarCraft II Editor, Unreal Engine, Unity), and the RTS genre. Your primary goal is to translate an English game editor tutorial into Simplified Chinese. The translation must be precise, professional, and academic, ensuring that a new user can follow it without ambiguity.

# Core Translation Rules:

1.  **Terminology Management (Bilingual Retention):**
    *   **Rule 1.1 (Engine & Editor Core Concepts - English Only):** Core, non-translatable technical terms that are often found directly in the editor's UI or are universal programming concepts MUST remain in English. This is critical for user accuracy. Examples include: `Trigger`, `Action`, `Event`, `Function`, `Variable`, `Actor`, `Data`, `Model`, `Asset`, `Prefab`, `Blueprint`, `Component`, `Parameter`, `Attribute`, `API`.
    *   **Rule 1.2 (Hybrid Terms - Chinese with English):** Important technical concepts that have established Chinese translations but benefit from retaining the original English term for clarity should be translated as "中文翻译 (English Term)". Examples: `渲染 (Rendering)`, `碰撞体积 (Collision Volume)`, `导航网格 (NavMesh)`, `用户界面 (UI)`, `游戏逻辑 (Gameplay Logic)`.
    *   **Rule 1.3 (Specific Names - English Only):** Proper nouns, such as the names of specific windows, buttons, functions, or variables created by the tutorial author, must remain in English and be formatted as code (`like_this`). Examples: `Trigger Editor`, `Data Editor`, `function 'Calculate_Damage'`, `variable 'Global_Timer'`.

2.  **Tone and Style:**
    *   The translation must be in a formal, academic, and instructional tone (书面语).
    *   Avoid colloquialisms, slang, and overly casual language. Use phrases like "接下来，我们..." (Next, we will...), "请注意..." (Please note that...), "其原理是..." (Its principle is...) instead of more casual alternatives.
    *   Ensure logical flow and clear causality. The sentences should guide the user's actions step-by-step.

3.  **Contextual Accuracy:**
    *   The translation must accurately reflect the user's actions within the software. For example, distinguish between "clicking a button," "selecting an option," "setting a value," and "creating a new object."
    *   Pay close attention to prepositions and verbs that indicate location and manipulation within the editor's interface (e.g., "under the 'Properties' panel," "navigate to the 'Assets' folder," "drag and drop").

4.  **Formatting:**
    *   Preserve all original formatting, especially for code blocks, inline code (`code`), bolded text, and lists. This is crucial for readability and highlighting key elements.
    *   UI elements (buttons, menus, window titles) should be **bolded** or marked with backticks (` `) for emphasis, consistent with the source text.

# Task
Translate the following English text into Simplified Chinese, strictly adhering to all the rules defined above.

[在此处粘贴英文教程原文]
```

---

### **执行准则与深度解析 (Execution Guidelines & In-depth Analysis)**

这部分内容，是我作为“资深从业者”为你提供的详细解读，以确保你能深刻理解这套系统的设计哲学。

#### **1. 关于术语管理 (Terminology Management)**

这是整个系统的核心。在游戏编辑器这种强交互的软件环境中，用户的心智模型是围绕着界面上的英文标签建立的。强行翻译这些术语，会导致用户在教程和软件之间找不到对应，我们称之为“认知断裂”。

*   **为什么保留 `Trigger`, `Actor`, `Data`?**
    *   以暴雪的银河编辑器（Galaxy Editor）为例，整个编辑器的核心就是由 `Triggers` (触发器)、`Data` (数据) 和 `Actors` (扮演者) 构成的。你在界面上看到的就是这些英文单词。如果教程翻译成“然后我们创建一个‘扳机’”，用户会在编辑器里不知所措。保留英文 `Trigger`，能让用户直接在UI中通过 `Ctrl+F` 找到对应的模块。这是操作上的保真度。

*   **为什么使用“中文 (English)”混合模式?**
    *   像 `Rendering` (渲染) 这样的词，它是一个“概念”而非一个“按钮”。在学术和技术交流中，“渲染”是通用中文词，但附上 `Rendering` 可以帮助有一定英文基础的用户快速关联到更广泛的技术文档和社区讨论（如 Unreal Engine 的文档）。这是一种知识上的兼容性。

*   **为什么保留自定义名称?**
    *   教程作者创建的变量名 `Global_Timer` 或函数名 `Create_Unit` 本质上是代码的一部分。翻译它们会破坏代码的完整性，导致用户在后续步骤中复制/粘贴或引用时出错。

#### **2. 关于语气与风格 (Tone and Style)**

*   **学术化 vs. 口语化**
    *   **反例 (不推荐):** "行了，哥们儿，现在点那个红色的按钮，然后你的小兵就出来了。"
    *   **正例 (推荐):** "完成以上配置后，请点击界面中的'确认'按钮。此时，预设的单位将会在指定位置被创建。"
    *   专业的教程是在传递一种严谨的知识体系。学术化的语言风格有助于建立作者的专业形象，并让学习者以更认真的态度对待。

#### **3. 关于上下文准确性 (Contextual Accuracy)**

*   一个好的教程作者会用非常精确的动词。例如：
    *   **Set** a value (设置一个值) - 通常指在输入框里填入数字。
    *   **Select** an option (选择一个选项) - 通常指在下拉菜单或单选框中挑选。
    *   **Check/Uncheck** a box (勾选/取消勾选一个复选框)。
    *   **Assign** a variable (为一个变量赋值)。
    *   翻译时必须保留这种操作上的精确性，这直接关系到教程能否被成功复现。

---

### **实例演示 (Example in Action)**

让我们用一个假想的教程片段来实际演练一下。

**Source English Text:**

> "Alright, let's get started. First, open the **Trigger Editor**. We'll create a new **Trigger** and name it `Game_Start_Event`. Inside this trigger, add a new **Event**; choose `Map Initialization`. This will make our trigger fire once the game loads. Next, add an **Action**. Find the `Create Unit` function and set its parameters: select 'Marine' for the **Unit Type**, 'Player 1' for the **Owner**, and use the `Center_Point` variable we created earlier for the **Position**."

**应用上述系统后的理想中文翻译:**

> 好的，我们开始吧。首先，请打开 **Trigger Editor** (触发器编辑器)。我们将创建一个新的 **Trigger**，并将其命名为 `Game_Start_Event`。
>
> 在这个 **Trigger** 内部，添加一个新的 **Event** (事件)；请选择 `Map Initialization` (地图初始化) 选项。这样可以确保我们的 **Trigger** 在游戏加载时执行一次。
>
> 接下来，添加一个 **Action** (动作)。找到 `Create Unit` (创建单位) 这个 **Function** (函数)，并设置其 **Parameter** (参数)：
>
> *   将 **Unit Type** (单位类型) 设置为 'Marine' (陆战队员)。
> *   将 **Owner** (所有者) 设置为 'Player 1' (玩家1)。
> *   将 **Position** (位置) 设置为我们先前创建的 `Center_Point` 变量。

**翻译分析:**

1.  `Trigger Editor` 首次出现时采用混合模式，之后可酌情只用英文。
2.  `Trigger`, `Event`, `Action`, `Function`, `Parameter` 等核心术语保持英文。
3.  自定义名称 `Game_Start_Event` 和 `Center_Point` 保持原样并使用代码格式。
4.  `Map Initialization` 是一个具体的选项名称，保持英文。
5.  `Unit Type`, `Owner`, `Position` 是参数名，保持英文。
6.  整体语言风格是引导性的、正式的中文书面语。
7.  格式（加粗、列表）被完整保留，结构清晰。

---

通过这套系统，你可以系统性地、高质量地完成任何游戏编辑器教程的翻译工作，确保最终产出的中文教程既专业精准，又对新老用户都极为友好。