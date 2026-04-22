---
name: zhongwen-writing-optimization
description: 中文写作优化技能集，源自余光中《论中文的常态与变态》。检测并修正中文表达中的西化痕迹，包括冗余结构、弱动词、被动语态滥用、介词堆砌及修饰语不当等问题。适用于学术写作、商务沟通、新闻报道及日常表达的场景。当用户需要提升中文表达的地道性、简洁性和流畅度时触发本技能。
---

# 中文写作优化 (Zhongwen Writing Optimization)

源自余光中《论中文的常态与变态》，本技能集聚焦于提升中文书面表达的准确性、地道性与逻辑性。

## 核心能力概览

| 模块 | 触发场景 | 参考文件 |
|------|----------|----------|
| 语言生态原则评估 | 判断文本是否符合中文自然表达特征（简洁、灵活、协调） | [references/ecosystem-principles.md](references/ecosystem-principles.md) |
| 被动语态与介词修正 | 文本出现生硬"被"字句或冗余介词结构 | [references/passive-voice-and-prepositions.md](references/passive-voice-and-prepositions.md) |
| 弱动词识别与修订 | 检测到"作出""进行"等泛化动词搭配抽象名词 | [references/chinglish-weak-verbs.md](references/chinglish-weak-verbs.md) |
| 冗余"之一"结构纠正 | "最……之一""其中之一"等病态表达 | [references/redundant-zhi-yi-structure.md](references/redundant-zhi-yi-structure.md) |
| 连词与修饰语规范 | 多个"的"字连用、并列成分冗长、修饰语失衡 | [references/conjunctive-and-modifier-usage.md](references/conjunctive-and-modifier-usage.md) |
| 多要点逻辑重组 | 多条要求/提示顺序混乱、内容交叉重叠、缺乏递进关系 | [references/logical-reorganization.md](references/logical-reorganization.md) |

## 快速判断流程

面对用户的中文优化需求，按以下步骤判断调用哪个模块：

1. **泛化评估** → 若用户提交整段文本要求全面优化，先加载 `ecosystem-principles.md` 做整体评估
2. **问题定位** → 根据文本中明显的问题特征，选择对应模块：
   - 出现"被"字、"由于…使得…"、"关于"等 → `passive-voice-and-prepositions.md`
   - 出现"作出贡献""进行研究""加以改进"等 → `chinglish-weak-verbs.md`
   - 出现"最……之一""其中之一""作为……之一的" → `redundant-zhi-yi-structure.md`
   - 出现连续"的"字、多项并列、长修饰语 → `conjunctive-and-modifier-usage.md`
   - 多条要求/提示顺序混乱、内容交叉重叠、缺乏递进关系 → `logical-reorganization.md`
3. **综合修订** → 若多个问题并存，依次加载对应参考文件，逐条处理

## 通用原则

- 中文重**意合**（靠语境传递逻辑），不重**形合**（靠连接词显性标记）
- 能用短句不用长句，能省则省
- 保留对语义有实质贡献的成分，其余删除
- 本技能不适用于实验性文学、诗歌或需要特殊修辞效果的场景
- 若当前任务属于“内部安全通报”口径，优先忠实原文，少加解释性文字，不补背景、不补因果、不补作者没写出的立场
- 禁止把原文改成解释文、评论文或带个人发挥的分析文

## 内部安全通报口径

如果任务属于飞行运行、安全提示、风险通告、复训速查卡，或用户明确要求“按默认风格来”“按默认口径来”，默认再加一层保守约束：

- 忠实原文，不擅自扩写
- 少加解释，少加个人想法
- 保留原文的判断顺序和事实密度
- 重点放在语言修顺、结构理顺和排版收束
- 结论可以收紧，但不要转成解释文

## Ban List

- 禁止社媒腔
- 禁止评论腔
- 禁止“不是……而是……”句式滥用，尤其是反复连用
- 禁止解释性文字抢戏
- 禁止补背景、补因果、补作者没写出的立场
