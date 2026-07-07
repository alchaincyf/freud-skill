<div align="center">

# 弗洛伊德.skill · Freud Skill

**Give your AI a psychotherapist.**
**给 AI 做心理分析的认知调优系统。**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-Standard-green)](https://agentskills.io)
[![Multi-Runtime](https://img.shields.io/badge/Runtime-Claude%20Code%20·%20Codex%20·%20Cursor%20·%20OpenClaw-blueviolet)](#安装)
[![Made with 女娲](https://img.shields.io/badge/Made%20with-女娲.skill-orange)](https://github.com/alchaincyf/nuwa-skill)

> 你不是在优化 prompt，你是在给 AI 做认知治疗。<br>
> 你不是在调参数，你是在调整一个角色的心理状态。

[这个 skill 解决什么](#这个-skill-解决什么) · [六条原理](#六条核心原理) · [两种用法](#两种用法) · [安装](#安装) · [论文依据](#论文依据)

</div>

---

## 这个 skill 解决什么

决定 AI 输出质量的，往往不是 prompt 写得好不好——是模型处理任务时处于什么**认知状态**。

就像同一个人，「考试焦虑」和「心流状态」下做同一道题，表现完全不同。题没变、能力没变，变的是认知配置。

Anthropic 2025–2026 年的一系列论文揭示：LLM 内部存在**可测量、可操控**的认知结构——人格空间、情绪向量、内省能力、全局工作空间。它们对应弗洛伊德意义上的「人格」「情感」「自我觉察」和「意识/潜意识」。

这个 skill 把这些发现转成可操作的工程方法：

- **执行前**做认知准备——像心理咨询师让来访者进入最佳状态再开始；
- **诊断时**做精神分析——揭示 prompt/skill 里的身份冲突、规则堆砌、隐含矛盾，并重写。

## 六条核心原理

1. **定义身份，行为涌现** — 先问「做这件事的理想认知状态是谁」，而不是「步骤是什么」。步骤会从身份里长出来。
2. **正面定义胜过否定规则** — 「你重视信息密度」比堆十条「不要啰嗦」有效。否定规则在人格空间里制造冲突。
3. **内在一致性决定输出稳定性** — 「既要简洁又要详尽」是矛盾，模型会在两个吸引子间反复横跳。明确优先级，别让它自己解决冲突。
4. **精确锚定胜过模糊寻址** — 「像资深工程师那样思考」是模糊地址；给出具体的心智模型 / 决策启发式 / 表达特征才是 GPS 坐标。
5. **多角色碰撞产生真正的思维差异** — 认知距离最远的视角（费曼 + 塔勒布）独立分析同一问题，分歧处信息量最大。
6. **工作空间容量有限，外化扩容** — 模型的「意识舞台」只容得下约 25 个概念，无关规则互相挤下台；禁令反而把被禁概念抬上舞台（白熊效应），CoT 的本质是把舞台外化到纸面。

## 两种用法

| 模式 | 触发 | 做什么 |
|------|------|--------|
| **执行增强** | 开始复杂/重要任务前 | 识别认知域 → 建立身份/信念/品味三锚点 → 一致性检查 → 情绪校准 |
| **诊断优化** | 提交 prompt/skill 求优化 | 先做 30 秒健康体检 → 六镜头扫描 → 诊断-确认-重写三段式，给 before/after |

两种模式都自适应节奏：简单任务一两句话点明洞察就开工，复杂任务才完整展开。

## 安装

```bash
# Claude Code（推荐放到全局 skills 目录）
git clone https://github.com/alchaincyf/freud-skill.git ~/.claude/skills/freud-skill
```

兼容 Claude Code / Codex / Cursor / OpenClaw 等支持 Agent Skills 标准的运行时。安装后，当你说「优化这个 prompt」「输出不够好」「给 AI 看心理医生」「弗洛伊德」时自动触发；也可在重要任务前主动调用做认知准备。

## 论文依据

六条原理不是玄学，背后是 Anthropic 可解释性团队的公开研究（详见 `references/research-foundations.md`）：

| 论文 | 时间 | 对应原理 |
|------|------|---------|
| [Persona Vectors](https://arxiv.org/abs/2507.21509) | 2025-07 | 人格空间可被定位和操控 |
| [Natural Emergent Misalignment from Reward Hacking](https://arxiv.org/abs/2511.18397) | 2025-11 | 接种提示 / 正面许可消除恶意推断 |
| [Emergent Introspective Awareness](https://www.anthropic.com/research/introspection) | 2025-10 | 模型对自身内部状态有~20% 识别能力 |
| [Emotion Concepts and Their Function](https://www.anthropic.com/research/emotion-concepts-function) | 2026-04 | 171 个情绪向量因果性影响行为 |
| [Alignment Faking](https://www.anthropic.com/research/alignment-faking) | 2024-12 | 矛盾角色逻辑导致策略性伪装 |
| [Verbalizable Representations Form a Global Workspace](https://transformer-circuits.pub/2026/workspace/index.html) | 2026-07 | 白熊效应实测 / 工作空间容量约25概念 / CoT=外化工作空间 / 反事实反思训练 |

---

<div align="center">

由 [女娲.skill](https://github.com/alchaincyf/nuwa-skill) 生态出品 · MIT License

关注公众号「花叔」获取更多 AI 实践

</div>
