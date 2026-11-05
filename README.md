# 测试用例专家（Test Case Expert）

面向软件测试与质量验证的通用 Agent Skill。先识别被测对象、测试目标和证据，再按风险选择测试层级、维度与方法，输出可执行的用例、覆盖映射和待确认事项。

本仓库按 [Agent Skills](https://agentskills.io/specification) / GitHub `gh skill` 约定组织：技能本体在 `skills/test-case-expert/`。

## 安装

```bash
gh skill install debraday885-lab/test-case-expert
```

或：

```bash
npx skills add debraday885-lab/test-case-expert
```

手动安装时，把 `skills/test-case-expert/` 整个目录放到目标 Agent 的 Skills 目录，并保留 `SKILL.md`、`references/`、`templates/` 的相对关系。

## 使用示例

- `$test-case-expert 帮我为这个功能设计测试用例。`
- `$test-case-expert 测试一下这个 Python 脚本，重点看输入边界和异常处理。`
- `$test-case-expert 帮我测试这个 Skill 的触发和多轮行为。`
- `$test-case-expert 审核这份测试用例，指出重复、遗漏和不可执行项。`
- `$test-case-expert 根据这份执行记录总结测试结果，并归并发现的问题。`

也可自然描述目标，例如“上线前帮我看看这个流程还要检查什么”。纯知识问题会直接解释，不强制进入用例生成。

## 仓库结构

```text
LICENSE
README.md
skills/test-case-expert/
  SKILL.md
  LICENSE
  README.md
  references/
  templates/
```

## 来源与许可

本 Skill 为作者原创。本包按 MIT License 授权，版权声明见根目录 `LICENSE`（Copyright (c) 2026 debraday885-lab）。
