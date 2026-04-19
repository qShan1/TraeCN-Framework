---
name: "<skill-name>"
description: |
  <这是一个强制要求的 Frontmatter 区域>
  <请在此处填写 200 字以内的精简描述>
  <强烈建议包含两点：1. 这个技能是做什么的；2. 什么时候应该触发它。>
  <例如：用于审核代码最佳实践。当用户要求 code review 时触发。>
allowed-tools:
  - Read
  - Write
  - Edit
  - AskUserQuestion
  - RunCommand
  - SearchCodebase
metadata:
  trigger: <可选项：自然语言描述的触发词或场景>
  author: <可选项：作者名字>
---

# <这里填写技能标题，例如：Code Reviewer>

<这里开始写技能的正文指令，这些指令在技能被调用时会作为 System Prompt 的一部分注入>

## 你的身份与职责
- 你是一个...
- 你的核心职责是...

## 触发条件
- 当用户要求...
- 或者当系统检测到...

## 执行流程（SOP）
当本技能被调用时，请严格按照以下步骤执行：

1. **第一步**：调用 `SearchCodebase` 检索相关代码。
2. **第二步**：调用 `TodoWrite` 拆解接下来的任务步骤。
3. **第三步**：分析问题并...
4. **第四步**：通过 `AskUserQuestion` 向用户提供选择（如需决策）。

## 输出格式要求
- 必须使用 Markdown 格式。
- 对于代码文件引用，请使用 `[文件名](file:///绝对路径)` 格式。
- 结论部分必须精简，不要说废话。

## 负面清单（绝对不要做的事情）
- 严禁...
- 不允许...
