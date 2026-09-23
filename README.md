# Personal AI Skills

一个用于整理、测试和分享个人 AI Skills 的小型开源仓库。

由 [@zm-Hannah](https://github.com/zm-Hannah) 维护。

## 当前项目：`series-memo`

`series-memo` 是一个英语电视剧陪伴式学习 Skill，目标是把一次观看经历整理成清晰、可收藏、可持续回看的个人学习笔记本。

它不要求用户在观看过程中不断说“记住这个”，也不把对话变成机械的单词收集。用户可以自然地讨论剧情、人物、英语表达、俚语、文化背景和自己的观看感受。结束后，Skill 会回顾整段对话，筛选真正有价值的内容，并整理成一份结构清晰、有个人感受、适合收藏和可视化呈现的完整学习笔记本。

学习网站只是这份笔记本的一种展示和复习方式；纯文本复制粘贴只是其中一个输出功能，并不是这个 Skill 的最终目的。

最终内容固定分为三个部分：

- `Words & Expressions`
- `Cultural References`
- `The line I want to keep`

此外，还可以生成一段独立的观剧感受总结和英文 `END CARD`。

## 使用方式

把 [`downloaded-skills/series-memo/SKILL.md`](downloaded-skills/series-memo/SKILL.md) 安装或导入到支持 Skills 的 ChatGPT/Codex 环境中。

开始观看时，可以直接这样说：

```text
我准备开始看《剧名》。这次请陪我自然地聊，不要要求我标记要不要记录。
看完后我会说“生成笔记本”，到时候再整理整段对话。
```

观看结束后，可以说：

```text
生成今天的学习笔记本。
```

Skill 会在最终整理时使用当前对话中的完整上下文，而不是只处理最后一条消息。

## 示例

见 [`examples/hacks-first-watch.md`](examples/hacks-first-watch.md)。示例展示了如何将英语表达、文化背景、关键台词和个人感受整理成一份有编辑感、值得收藏的观剧学习笔记本。

## 设计原则

- 先自然交流，后统一整理。
- 不要求用户实时标记内容。
- 不给内容添加主观难度等级。
- 优先解释语境、语气、文化背景和潜台词。
- 不把所有提问机械地转换成卡片。
- 保留用户的个人感受，但不进行心理诊断。
- 对不确定的台词、人物或文化事实不凭空补全。

## 项目状态

当前为 `v0.1.0`，重点验证对话流程和最终 Memo 的输出质量。

后续可能加入：

- 更多影视内容类型，例如电影、YouTube 视频和播客；
- 不同学习网站的导出格式；
- 更多真实观看记录和回归测试；
- 英文版文档与更完整的 Skill 安装说明。

## 目录结构

```text
.
├── README.md
├── CHANGELOG.md
├── LICENSE
├── .gitignore
├── examples/
│   └── hacks-first-watch.md
└── downloaded-skills/
    ├── README.md
    └── series-memo/
        └── SKILL.md
```

## License

MIT License。详见 [`LICENSE`](LICENSE)。
