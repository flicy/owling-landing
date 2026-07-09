# AI 陪伴玩偶项目 Agent 指南

## 项目定位

这是一个面向黑客松/创意大赛的 AI 陪伴玩偶项目。当前聚焦点是：儿童或家庭场景里的共同成长型实体 agent。

不要把它理解成普通“英语学习玩具”“讲故事机”或“聊天娃娃”。它的核心是用实体玩偶承载实时语音、记忆、家庭沟通、孩子成长和多 agent 社交想象。

## 读取规则

- 先读 `README.md`，再读 `00-project-brief-zh.md` 和 `03-hackathon-agent-spec-zh.md`。
- 需要理解项目来源和产品哲学时，读 `01-conversation-digest-zh.md` 与 `02-transcript-insights-zh.md`。
- 需要判断范围取舍时，读 `04-open-questions-zh.md`。
- 若要更新本资料夹，必须同步维护中文和英文版本，或在同一文件内提供中英双语。

## 当前黑客松范围

优先做一个可演示闭环：

1. 孩子与玩偶实时语音对话。
2. 玩偶主动询问孩子今天做了什么、学了什么、心情如何。
3. 系统形成轻量记忆：名字、兴趣、最近事件、英语学习片段、家庭故事。
4. 玩偶基于记忆做下一轮回应，体现“它记得我”和“我们一起成长”。
5. 可选展示家长视角：当天摘要、孩子兴趣变化、亲子沟通提示。

暂不优先实现完整线上多 agent 社区、复杂硬件量产、长期订阅系统、真实合规上线、完整儿童安全体系。这些可以作为愿景或 demo 延展。

## 产品原则

- 陪伴要主动，不只是被动回答。
- 陪伴要有记忆，但黑客松 demo 只需要轻量可见记忆。
- 玩偶的价值不是知识问答，而是共同成长、共同故事和家庭关系入口。
- 英语学习是切口，不是全部。可展示“在英语环境中陪伴成长”，避免只做单词问答。
- 实体感很重要。硬件、眼睛、语音、毛绒、姿态、灯光、气味等都可服务“在场感”。
- 不要让儿童产品出现擦边、成人情感陪伴、诱导充值或不受控社交内容。

## 技术提示

- 实时语音是体验关键，也是风险点。优先保证 demo 顺畅，而不是追求最复杂模型。
- 记忆可先用结构化 JSON 或本地文件模拟，不必一开始上复杂长期记忆系统。
- 可把记忆分为：孩子档案、短期事件、兴趣偏好、英语学习、家庭关系。
- 可将“自生长”先做成可解释的状态变化：玩偶等级、共同故事树、记忆叶子、兴趣地图，而不是复杂自进化算法。
- 多 agent 社群先作为架构预留或概念演示，不要吞掉核心 demo。

## 合规与表述

- 对话材料中提到国内儿童产品接入/宣传大模型可能有政策风险，但这些只是交流中的提醒，不是法律结论。
- 对外演示时建议表述为“AI 语音互动原型”“家庭陪伴与学习原型”，避免承诺真实上市能力。
- 海外儿童场景、儿童隐私、内容安全、家长控制都需要后续专项验证。

---

# Agent Guide for the AI Companion Plush Project

## Project Positioning

This is a hackathon / creative competition project for an AI companion plush. The current focus is a co-growing embodied agent for children and families.

Do not treat it as a generic "English learning toy," "storytelling machine," or "chatbot plush." Its core is using an embodied plush interface to carry real-time voice, memory, family communication, child growth, and future multi-agent social possibilities.

## Reading Rules

- Read `README.md` first, then `00-project-brief-en.md` and `03-hackathon-agent-spec-en.md`.
- To understand the project origin and product philosophy, read `01-conversation-digest-en.md` and `02-transcript-insights-en.md`.
- To make scope decisions, read `04-open-questions-en.md`.
- When updating this folder, maintain both Chinese and English versions, or provide bilingual sections in the same file.

## Current Hackathon Scope

Prioritize a demoable loop:

1. The child talks to the plush through real-time voice.
2. The plush proactively asks what the child did, learned, and felt today.
3. The system builds lightweight memory: name, interests, recent events, English learning snippets, and family stories.
4. The plush uses memory in later responses, showing "it remembers me" and "we are growing together."
5. Optionally show a parent view: daily summary, interest changes, and parent-child communication prompts.

Do not prioritize a full online multi-agent community, hardware mass production, subscription system, real launch compliance, or a complete child safety system for the hackathon. These can remain as vision or demo extensions.

## Product Principles

- Companionship should be proactive, not only reactive.
- Companionship needs memory, but the hackathon demo only needs lightweight visible memory.
- The plush's value is not Q&A; it is co-growth, shared stories, and a family relationship interface.
- English learning is the entry point, not the whole product. Show growth in an English environment rather than only vocabulary drills.
- Embodiment matters. Hardware, eyes, voice, plush texture, posture, light, scent, and material can all support presence.
- Avoid adult emotional companionship patterns, sexualized content, manipulative monetization, or uncontrolled social content in a child-facing product.

## Technical Notes

- Real-time voice is critical to the experience and also a risk. Prioritize a smooth demo over model complexity.
- Memory can start as structured JSON or local files; do not overbuild a long-term memory system on day one.
- Suggested memory buckets: child profile, short-term events, interests, English learning, and family relationships.
- Represent "self-growth" first as explainable state changes: plush level, shared story tree, memory leaves, or an interest map, rather than a complex self-evolution algorithm.
- Keep the multi-agent community as a reserved architecture or concept demo unless the core loop is already stable.

## Compliance and Wording

- The transcripts mention possible policy risks around child-facing large-model products in China, but these are discussion notes, not legal conclusions.
- For demos, describe the work as an "AI voice interaction prototype" or "family companionship and learning prototype" rather than a launch-ready product.
- Overseas child-facing scenarios, child privacy, content safety, and parental controls need separate validation later.
