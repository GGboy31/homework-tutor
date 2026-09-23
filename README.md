# Homework Tutor · 课程作业辅导

一个面向 Codex 的作业辅导插件。优先采用课件的方法，结合教材与题目数据，提供可追溯的解答和追问讲解。

## 功能

- 支持教材题号、作业文件、照片、截图及组合题源。
- 分开管理解题方法与参数来源，核对单位、近似和适用条件。
- 支持完整解答、提示、答案检查和概念追问。
- 默认对话输出；按需将 Markdown 保存到作业目录，内置公式空行规范。

## 使用

安装后，在新的 Codex 任务中使用 `$homework-tutor`，例如：

> 使用 $homework-tutor，按照本项目的课件解答作业第 2 题；题外参数优先查教材，注明来源。

> 我没看懂这一题为什么能忽略空穴项，请结合课件解释。

将课件、教材和作业保存在当前工作区，或提供题目图片。插件不附带课程教材、学生作业或私人聊天记录。

## 文件结构

- `.codex-plugin/plugin.json`：插件清单。
- `skills/homework-tutor/SKILL.md`：核心流程。
- `skills/homework-tutor/references/markdown-math.md`：Markdown 与公式约定。
- `skills/homework-tutor/agents/openai.yaml`：技能显示与调用设置。

也可将 `skills/homework-tutor` 文件夹复制到个人 Codex 的 `skills` 目录作为独立 skill 使用；避免同时安装两份造成重复。

## 开源与贡献

采用 MIT 许可证。你可以使用、修改和分发自己的副本。原仓库由维护者管理；欢迎通过 Issue 或 Pull Request 提建议，外部贡献不会自动合并。
