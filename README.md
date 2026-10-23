# Humanizer Stop-Slop Skill

融合 **stop-slop** 与 **humanizer-zh** 的大一统文本深度润色 Skill。

## 核心设计：双阶段流水线

润色任何文本时，系统按顺序执行：
1. **阶段一（Stop-Slop 结构剪枝）**：剥离清嗓开场、多余副词、二元对立（不是A而是B）、虚假拟人、戏剧化碎片句式与做作节奏。
2. **阶段二（Humanizer-zh 语感精修与事实铁律）**：清洗中式AI腔、层叠的“的”、“进行+动词”、被字句滥用、四字同义堆叠，并施加最严格的事实保真（绝不臆造任何未提供的数据或事实，严格锁定确定性）。
3. **阶段三（交付前核对）**：事实与边界清单核查，输出自然干净的人话终稿。

## 目录结构

- `SKILL.md`：核心工作流与双阶段操作规范。
- `references/stop-slop-phrases.md`：需剔除的词组、黑话、清嗓词与副词清单。
- `references/stop-slop-structures.md`：需规避的公式化句式结构与节奏套路。
- `references/humanizer-zh-patterns.md`：31 项中文细分表达模式与修改边界。
- `references/examples.md`：润色前后对照范例库。
