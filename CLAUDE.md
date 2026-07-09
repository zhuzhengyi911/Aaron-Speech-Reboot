# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Aaron Speech Reboot** 是一个 Obsidian 笔记库，用于系统化学习英语口语。核心方法是 **AI 场景驱动**：针对真实生活场景（如在外就餐、订酒店、代码评审等），用 AI 生成地道口语对话，配合英语 Pod 和 YouTube 等真实语料，逐步积累可复用的口语表达。

**最终目标**：在各种真实场景下能自然、流利、地道地用英语交流，听力秒反应，表达无卡顿，遇到突发情况能自救。

## Project Structure

```
├── 00-索引/
│   └── 场景目录总览.md              # 所有场景的分类索引和完成状态
├── 01-场景笔记/
│   └── [场景名称]/
│       ├── 00-[场景名称]-总览.md     # 子场景列表（表格）
│       ├── 01-子场景A.md            # 每个子场景一个文件，包含对话+语言点
│       ├── 02-子场景B.md
│       └── ...
├── 02-语料库/
│   ├── English-Pod原文/             # English Pod 原始听力素材
│   ├── Ariannita La Gringa/         # YouTube 频道语料
│   └── 食物名词大全.md               # 分类词汇表（按餐厅类型/食材分类）
└── 98-每日学习记录/
    └── README.md                    # 每日学习摘要，供 AI 复习回顾
```

## 场景笔记写作范式

每个场景笔记文件遵循以下格式：

```markdown
# 子场景名称

## 对话 N：场景描述

**A (顾客):** 对话内容...  
**B (餐厅):** 对话内容...

> **语言点**
> - **表达** — 中文解释
```

**关键规则**：
- 对话以顾客视角为主（A = 顾客/学习者，B = 服务员/对方）
- 每个子场景覆盖：正常流程 + 突发情况 + 委婉/礼貌表达
- 语言点紧跟在对话下方，用 blockquote 引用格式
- 可扩展部分用 `> **扩展：**` 标记

## 常用操作

### 新建一个场景
1. 在 `01-场景笔记/` 下创建场景文件夹（如 `订酒店/`）
2. 创建 `00-订酒店-总览.md`，列出所有子场景表格
3. 逐个创建子场景文件（`01-xxx.md`, `02-xxx.md`...）
4. 更新 `00-索引/场景目录总览.md`

### 添加语料
- English Pod 原文放在 `02-语料库/English-Pod原文/`
- 其他视频/音频语料建独立目录（如 `Ariannita La Gringa/`）
- 词汇表放在 `02-语料库/` 根目录

### 每日记录
在 `98-每日学习记录/README.md` 追加一条当日学习摘要。

## Useful Commands

- **View in Obsidian**: 在 Obsidian 中打开 `/Users/aaron/Aaron-Speech-Reboot` 查看渲染效果
- **Git**: 标准 git 操作（`git add`, `git commit`, `git push`）
- `.obsidian/` 已被 gitignore 排除，不提交
