# zlc-writing

按 Luocheng Zhang 的写作偏好，撰写、润色和审查机器学习与计算机视觉论文，整理 LaTeX 主稿及投稿材料。默认中文讨论、英文论文写作，并优先遵守用户当前要求和项目 `AGENTS.md`。

## 核心约定

- 摘要不报告具体实验数值、提升百分比、参数量或具体实验配置；具体数据保留在正文、表格和补充材料。
- 从实际问题、方法机制与证据组织论证，核实文献和实现，不编造结果或作者事实。
- 引言以贡献列表结束；常规实验验证不单独作为创新点；相关工作最多分为三个主题。
- 保留主稿必要细节，检查表格、段落断行、浮动图表、参考文献和异常留白。
- 润色请求不自动授权运行实验；投稿材料准备不等于已完成投稿。

完整规则见 [SKILL.md](SKILL.md)。公开版本不包含特定论文的作者分工、实验记录及本机路径。

## 安装

在 Codex 中使用内置 skill-installer：

```text
使用 skill-installer 从 https://github.com/GO-1-Z/zlc-writing 安装这个 skill。
```

也可以将本仓库克隆到 Codex 的个人 skills 目录；下列示例适用于未设置自定义 CODEX_HOME 的环境，且目标目录必须不存在：

```bash
git clone https://github.com/GO-1-Z/zlc-writing.git ~/.codex/skills/zlc-writing
```

如果本机已安装同名 skill，先备份并比较内容，避免覆盖个人定制。安装后若未显示，重启 Codex 再检查。

## 使用示例

```text
使用 $zlc-writing 润色当前论文的摘要和引言，保留实验事实，直接修改有依据的文字问题。
```

```text
使用 $zlc-writing 检查当前 LaTeX 主稿的叙事和排版，并列出需要作者确认的事实或新增实验。
```

## 文件

```text
zlc-writing/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── README.md
```

本 skill 保存写作工作流与个人偏好，不附带模型权重或特定论文稿件。
