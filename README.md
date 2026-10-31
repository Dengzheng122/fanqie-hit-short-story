# fanqie-hit-short-story

<p align="center">
  <a href="https://github.com/tianyayu6/fanqie-hit-short-story/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/tianyayu6/fanqie-hit-short-story?style=for-the-badge&logo=github" /></a>
  <a href="https://github.com/tianyayu6/fanqie-hit-short-story/network/members"><img alt="Forks" src="https://img.shields.io/github/forks/tianyayu6/fanqie-hit-short-story?style=for-the-badge&logo=github" /></a>
  <a href="https://github.com/tianyayu6/fanqie-hit-short-story/issues"><img alt="Issues" src="https://img.shields.io/github/issues/tianyayu6/fanqie-hit-short-story?style=for-the-badge&logo=github" /></a>
  <a href="https://github.com/tianyayu6/fanqie-hit-short-story/commits/main"><img alt="Last commit" src="https://img.shields.io/github/last-commit/tianyayu6/fanqie-hit-short-story?style=for-the-badge&logo=git" /></a>
  <a href="LICENSE"><img alt="License" src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge" /></a>
</p>

你给一个核心梗，它把它扩成番茄短篇爆款流程：大纲、标题导语、12000字正文、编辑审稿、重写、去AI味终稿。

```bash
npx skills add tianyayu6/fanqie-hit-short-story
```

## 它解决什么问题

写番茄短篇最容易卡在三件事。

梗有了，但不知道怎么排成8-10章。

正文能写出来，但节奏慢、爽点散、开篇不抓人。

AI稿看起来很完整，却有空泛比喻、模板金句和不像真人写的口吻。

这个 skill 把流程固定下来：先按番茄短篇口味做结构，再按短篇编辑视角审稿，最后做去AI味处理，并用一句一行交付最终稿。

## 能生成什么

- 根据核心梗生成8-10章短篇爆款大纲
- 生成小说标题、导语和正文
- 正文目标为每章约1000-1200字，全文不少于12000字
- 用短篇编辑视角审稿，指出结构、节奏、爽点、虐点和AI味问题
- 根据审稿意见重写全文
- 删除空洞比喻和套话，输出一句一行终稿
- 在需要时展示参考过的公开来源和方法论

## 示例输入

你可以直接这样说：

- "用番茄爆款短篇写这个梗：真千金回家当天，弹幕告诉我全家都会害死我。"
- "把这个核心梗扩成12000字番茄短篇，最后一句一行。"
- "先给我大纲，再写正文，写完按短篇编辑审稿重写。"
- "说明你参考了哪些公开爆款方法论。"

## 工作流程

1. 拆解核心梗：类型、情绪主轴、主角、对手、爆点装置。
2. 生成8-10章大纲：每章包含事件、情绪价值、反转和结尾钩子。
3. 生成标题和导语：标题直给卖点，导语3-5段抓冲突。
4. 写正文初稿：默认10章，全文不少于12000字。
5. 编辑审稿：检查开篇、人物主动性、反转密度、情绪兑现和逻辑。
6. 重写全文：根据审稿意见重构，不只做局部润色。
7. 去AI味终稿：删空话、换具体动作、保留人物口吻，并一句一行。

## 方法论来源

方法论写在 `references/source-notes.md`，包括番茄官方短篇说明、番茄短故事激励计划、公开榜单样本、网文生态报道和用户提供截图中的爆款分析。

这个 skill 只学习公开作品的结构、节奏、题材组合和情绪兑现方式。

它不会复制、洗稿、替换人名改写或续写任何已有作品。

## 前置要求

- [ ] 已安装支持 Agent Skills 的工具，例如 Codex、Claude Code 或其他兼容工具。
- [ ] 已安装 Node.js 和 `npx`，可运行 `npx --version`。
- [ ] 能访问 GitHub，安装时可拉取公开仓库。
- [ ] 使用时提供一个原创核心梗，而不是要求改写已有小说。

## 安装

1. 运行安装命令：

```bash
npx skills add tianyayu6/fanqie-hit-short-story
```

2. 验证能发现 skill：

```bash
npx skills add tianyayu6/fanqie-hit-short-story --list
```

3. 在你的 agent 里用自然语言触发：

```text
用 fanqie-hit-short-story，把这个核心梗写成番茄爆款短篇。
```

## 文件结构

- `SKILL.md`：主流程和硬约束。
- `references/methodology.md`：番茄爆款短篇结构、标题、导语、章节节奏。
- `references/editorial-and-deai.md`：短篇编辑审稿清单和去AI味规则。
- `references/source-notes.md`：公开来源和方法论摘记。
- `agents/openai.yaml`：Codex 界面元数据。

## 限制

- 不保证真实商业爆款结果，只提供可执行的爆款化写作流程。
- 不适合仿写、洗稿、续写平台已有作品。
- 一次输出12000字以上正文可能受上下文长度影响，需要让 agent 分批继续。
- 公开来源的榜单数据会变化，长期使用时建议定期更新 `source-notes.md`。

## Troubleshooting

| 问题 | 原因 | 解决方法 |
| --- | --- | --- |
| `npx skills add` 找不到 skill | GitHub 仓库还没同步或网络访问失败 | 稍后重试，或先运行 `npx skills add tianyayu6/fanqie-hit-short-story --list` |
| 触发后没有读取方法论 | agent 没识别到 skill 名 | 明确说“使用 fanqie-hit-short-story”或“使用番茄爆款短篇 skill” |
| 正文少于12000字 | 单次回复长度不足 | 要求继续生成下一批，并保持同一大纲和字数台账 |
| 输出不是一句一行 | 终稿阶段未执行格式要求 | 要求“只输出去AI味终稿，一句一行” |
| 内容太像AI | 初稿未经过审稿重写 | 要求先给短篇编辑审稿意见，再按意见重写全文 |

## License

MIT
