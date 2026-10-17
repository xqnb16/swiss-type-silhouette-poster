# 安装与使用

展示名称：瑞士风文字剪影海报 Skill。技术标识：`swiss-type-silhouette-poster`。

## 标准技能包

1. 从仓库 releases 目录下载 `swiss-type-silhouette-poster-v0.1.0.zip`。
2. 解压得到同名技能目录，保留其中的 SKILL.md、references 和 agents。
3. 将完整目录放入宿主支持的技能目录，按宿主要求重新加载。不要仅复制 SKILL.md 后丢掉参考文件。
4. 让 Agent 使用此技能，并提供主题、品牌名、标语、颜色和构图参数。

Codex 本地安装可将完整目录放在 `~/.codex/skills/` 下。其他 Agent 的目录位置与导入方式，以宿主的官方说明为准。

支持 skills CLI 的环境也可运行：

```sh
npx skills add yangqiannb16-commits/swiss-type-silhouette-poster --skill swiss-type-silhouette-poster
```

## WorkBuddy 适配包

下载 `swiss-type-silhouette-poster-workbuddy-v0.1.0.zip`。这个包将 SKILL.md 放在根目录，包含版本、作者、展示名、中英文描述及参考文件提示。若当前 WorkBuddy 界面支持 ZIP 导入，可选择该包；若要求目录，则解压后按界面要求选择。此版本尚未完成实机导入验证。

## 直接复制

打开「瑞士风文字剪影海报-复制即用-v0.1.0.txt」，将全文复制进新对话或作为文件交给 Agent 读取。这个文件已经内嵌完整视觉规则与示例，不依赖外部参考文件。

仅加载文件不会自动生图。读取后，再提出具体的海报创作请求。没有生图工具的 Agent 会输出完整提示词，可再交给具备生图功能的工具。

## 填写参数

```text
主题物体：
品牌名：
品牌标语：
关键词：（可留空）
背景主色：
点缀色：
构图方式：A / B / C
辅助元素：无
```

A 为纵向，B 为横向或斜向，C 为居中对称。构图未填时可按物体形态推定。若希望 Agent 自行选择颜色或品牌文案，请明确授权；也可以明确不要品牌区。

## 校验文件

`releases/swiss-type-silhouette-poster-SHA256SUMS.txt` 记录两份 ZIP 与复制版文件的 SHA-256。下载后可与本地文件计算结果比对。
