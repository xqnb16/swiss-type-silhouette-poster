# 瑞士风文字剪影海报 Skill

把一个物体变成由密排微型英文文字构成的二维剪影，制作一张 3:4 竖版极简广告海报。基于用户提供的瑞士风文字剪影提示词整理，支持三种构图和后续定向修改。

## 能做什么

- A 纵向、B 横向或斜向、C 居中对称，按主题与指定构图组织画面。
- 微型英文文字填满主体轮廓；辅助元素按需使用网点剪影。
- 原样保留品牌名与标语的拼写、大小写和标点。
- 输入不全时只补问必要项；中文关键词可转换成英文。
- 有生图工具时调用宿主工具；没有时输出可复制的完整提示词。
- 改图时保留未指定修改的参数；可查看结果时检查画面并针对偏差修正。

## 下载

| 使用方式 | 文件 |
| --- | --- |
| 标准技能包 | [下载 ZIP](releases/swiss-type-silhouette-poster-v0.1.0.zip?raw=true) |
| WorkBuddy 适配包 | [下载 ZIP](releases/swiss-type-silhouette-poster-workbuddy-v0.1.0.zip?raw=true) |
| 完整复制版 | [查看并复制](releases/瑞士风文字剪影海报-复制即用-v0.1.0.txt) |
| 文件校验值 | [SHA256SUMS](releases/swiss-type-silhouette-poster-SHA256SUMS.txt) |

标准包包含独立技能目录；WorkBuddy 包将 SKILL.md 放在压缩包根目录。具体导入入口以各平台当前界面为准。无法导入 Skill 的聊天工具，可使用完整复制版。

## 安装

支持 skills CLI 的环境可运行：

```sh
npx skills add yangqiannb16-commits/swiss-type-silhouette-poster --skill swiss-type-silhouette-poster
```

也可下载标准包，将完整的 `swiss-type-silhouette-poster` 目录放入宿主支持的技能目录，保留 references 和 agents 子目录。更多方式见 [安装说明](INSTALL.md)。

## 开始使用

加载技能后，把下面的内容发给 Agent：

```text
请使用瑞士风文字剪影海报 Skill 制作一张海报。
主题物体：落地灯
品牌名：LUMINA
品牌标语：a brighter home for quieter evenings
关键词：light, home, calm, evening, shade, glow, balance, quiet
背景主色：深海军蓝 #1E3A8A
点缀色：明黄 #F5C518
构图方式：A
辅助元素：无
```

示例品牌仅用于演示，实际创作时替换为自己的文案。后续可以直接说：“背景改为深红，其他保持不变。”

## 使用边界与验证状态

Skill 本身不提供图像模型或 API 额度。生图与改图取决于所用 Agent 的实际工具；纯文本环境交付提示词。默认产物为有二维矢量视觉的图像，不承诺可编辑 SVG，也不能保证每个模型都准确生成文字。

版本：0.1.0。已检查文件结构、相对引用、UTF-8、ZIP 完整性及复制版内容一致性；尚未在 WorkBuddy 实机导入，也未对实际生图效果进行验收。

## 目录

```text
skills/swiss-type-silhouette-poster/
  SKILL.md
  agents/openai.yaml
  references/visual-spec.md
  references/examples.md
releases/
INSTALL.md
```

技术标识为 `swiss-type-silhouette-poster`，展示名称为「瑞士风文字剪影海报 Skill」。
