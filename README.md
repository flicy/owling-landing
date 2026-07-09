# 灵偶 OWLING

> 软硬件结合的英语学习玩伴，面向 3 岁到五年级，和小朋友一起自生长。

探月黑客松项目 · AI 创意大赛

---

## 在线预览

| 页面 | 链接 |
|------|------|
| V1 基础版 | https://flicy.github.io/cola-pages/owling/ |
| V2-A 故事树（暖色自然系） | https://flicy.github.io/cola-pages/owling-v2a/ |
| V2-B 宠物小精灵（暗色魔法系） | https://flicy.github.io/cola-pages/owling-v2b/ |
| Demo 体验入口 | http://mbp.liaoxingyi.com/ |

---

## 目录结构

```
owling-landing/
├── README.md
│
├── version-a-story-tree/
│   └── index.html              # V2-A：故事树隐喻（种子→树苗→大树→森林）
│
├── version-b-spirit-pet/
│   └── index.html              # V2-B：宠物小精灵隐喻（精灵蛋→孵化→进化→社交）
│
├── version-v1/
│   └── index.html              # V1：功能导向基础版
│
└── docs/
    ├── 00-project-brief-zh.md          # 项目简报：定位、用户、核心功能
    ├── 01-社媒文案.md                   # 小红书 + 朋友圈召集用户文案
    ├── 02-AI儿童陪伴硬件合规要点.md      # 国内外合规法案整理（中/美/欧）
    ├── 03-hackathon-agent-spec-zh.md   # 黑客松执行规格：Demo剧本、MVP清单、数据结构
    ├── 04-open-questions-zh.md         # 未决问题与验证点
    └── 视频脚本-灵偶角色介绍.md          # 角色介绍视频脚本（7/10 拍摄）
```

---

## 产品核心

**一句话**：一个能和孩子实时对话、记住 ta 每天的事、陪 ta 一起长大的毛绒玩偶。

**体验闭环**：语音对话 → 轻量记忆 → 成长可视化 → 家长摘要

**成长隐喻体系**：
```
故事树（整体容器）
  ├── 记忆叶子（每日内容单元，灵感来自「一日一叶」）
  ├── 兴趣地图（叶子聚合后的主题分布）
  └── 伙伴等级（多 Agent 社交层）
```

**产品架构**：
- 硬件端：毛绒玩偶（灵偶），孩子的对话入口
- 小朋友软件端：Pad / 儿童手表，展示记忆叶子、故事树、兴趣地图
- 家长软件端：APP 面板 + 主动提醒卡片/短信

---

## 协作

- 直接改对应目录下的 `index.html`
- 每个版本是一个 HTML（内联 CSS + JS）+ `assets/` 本地配图，无外部依赖
- 文档在 `docs/` 目录，随时补充更新
- PR 或直接 push 均可

---

## 技术栈

- 纯 HTML / CSS / JS，每版一个页面 + 本地 assets 配图，无外部 CDN 依赖
- AI 生成品牌配图（统一的猫头鹰玩偶形象，位于各版本 assets/ 目录）
- 系统字体栈（PingFang SC / Microsoft YaHei 等，国内访问无阻塞）
- IntersectionObserver 滚动动画（含 prefers-reduced-motion 与 noscript 降级）
- 响应式设计（移动端适配）
