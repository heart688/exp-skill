# Paper Experiment Story · 论文实验写作

把实验部分写成连续的主张与证据论证，让读者看懂每个实验为什么做、结果意味着什么。

这是一套可跨研究领域使用的 Agent Skill，覆盖实验框架、段内递进、小节衔接和 insight 写作。

## 它解决什么

- **框架：** 按核心主张安排实验，突出最有判别力的对照。
- **段落：** 用“问题 → 对照 → 观察 → insight”推进结果分析。
- **衔接：** 让上一节留下的问题自然引出下一节。
- **解释：** 区分性能、组件贡献、信息使用、机制与适用条件。
- **结论：** 保留真实例外，避免逐行复述图表或扩大证据范围。

## 开始使用

入口是 [SKILL.md](SKILL.md)。提供论文主问题、方法、实验协议及真实图表结果，再说明需要框架、改写还是审读。

```text
使用 $paper-experiment-story 重写实验部分。
先理顺每个小节回答的问题，再按问题、对照、观察和 insight 组织段落。
说明各实验怎样回应论文的核心判断，并自然衔接。
使用现有结果，保留真实例外与结论范围。
```

## 安装

在 Codex 中首次安装：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/heart688/exp-skill.git ~/.codex/skills/paper-experiment-story
```

其他支持 Agent Skills 的工具可按其安装方式使用。与其他写作 AI 配合时，提供 `SKILL.md` 及它链接的参考文件。此 skill 为纯文本，无需安装运行时依赖。

## 内容

```text
SKILL.md
agents/openai.yaml
references/paragraph-patterns.md
```

[段落与衔接模式](references/paragraph-patterns.md)覆盖总体结果、消融、干预、适用条件和效率分析，并附段内自检问题。

## 原则

实验服务于同一个研究判断。图表呈现数据，正文解释最关键的发现及其意义；观察、解释与已验证结论各自保持准确范围。小节顺序随论文调整。

需要先梳理全文主线时，可配合使用[论文故事 skill](https://github.com/heart688/insight-skill)。
