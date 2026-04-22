# zhongwen-writing-optimization

中文写作优化技能集。用于识别并修正中文表达里的西化痕迹、冗余结构、弱动词、被动句、介词堆砌、修饰语失衡，以及多要点文本的逻辑混乱问题。

这个 skill 不是单点润色器，而是一组可组合的中文优化模块。适合整段文本的整体诊断，也适合按问题类型选择单个参考模块逐项修订。

## 仓库内容

- `SKILL.md`：主 skill 说明、模块总览、触发判断和通用原则
- `references/ecosystem-principles.md`：中文自然表达的三大核心原则
- `references/passive-voice-and-prepositions.md`：被动句和介词滥用修正
- `references/chinglish-weak-verbs.md`：弱动词识别与改写
- `references/redundant-zhi-yi-structure.md`：冗余“之一”结构处理
- `references/conjunctive-and-modifier-usage.md`：连接词和修饰语规范
- `references/logical-reorganization.md`：多要点文本的逻辑重组

## 适用场景

- 学术写作、商务沟通、新闻报道、说明文
- 日常中文表达的地道化、简洁化和逻辑优化
- 用户提交整段文本，希望系统性优化中文表达
- 文本同时存在多种问题，不适合只靠单一规则处理

## 这个 skill 的特点

- 以“模块化诊断 + 对症修订”为核心
- 兼顾整体中文生态与具体语言病症
- 适合整段评估，也适合按症状精修
- 对“内部安全通报”这类任务内置保守口径约束

## 使用方式

1. 将 `SKILL.md` 放入你的 skill 目录。
2. 遇到整体中文优化任务时直接触发主 skill。
3. 若需要更细粒度处理，再按问题类型查阅 `references/` 下的对应模块。

## 适合发布的原因

- 结构清晰，主 skill 与参考模块边界明确
- 内容自洽，不依赖本地脚本或私有资源
- 可以单独使用，也可以作为中文写作优化 skill 集合的一部分
