# 灵偶 OWLING — 产品介绍页

AI 陪伴玩偶黑客松项目的产品介绍页源码。

## 两个版本

| 版本 | 设计方向 | 预览链接 |
|------|---------|---------|
| **V2-A 故事树** | 暖色自然系 · 种子→树苗→大树→森林 | [预览](https://flicy.github.io/cola-pages/owling-v2a/) |
| **V2-B 宠物小精灵** | 暗色魔法系 · 精灵蛋→孵化→进化→社交 | [预览](https://flicy.github.io/cola-pages/owling-v2b/) |

## 目录结构

```
owling-landing/
├── version-a-story-tree/
│   └── index.html          # A版：故事树隐喻
├── version-b-spirit-pet/
│   └── index.html          # B版：宠物小精灵隐喻
└── README.md
```

## 产品简介

灵偶是面向儿童和家庭的 AI 陪伴玩偶——能实时语音对话、记住孩子的日常、陪孩子共同成长的实体 Agent。

**核心体验闭环**：语音对话 + 轻量记忆 + 成长可视化 + 家长摘要

## 协作说明

- 直接修改对应版本的 `index.html`
- 每个版本是单文件 HTML（含内联 CSS + JS），无外部依赖
- 提 PR 或直接 push 到 main 均可
- Demo 入口链接指向：http://mbp.liaoxingyi.com/

## 技术栈

- 纯 HTML/CSS/JS，单文件
- Google Fonts (Inter)
- IntersectionObserver 滚动动画
- 响应式设计（移动端适配）
