# OpenCLI Skill Architecture（按领域分组）

这个目录用于构建 **面向 Agent 的 skill 文档体系**，解决“命令很多时，单一 SKILL.md 不够用”的问题。

## 设计目标

- `SKILL.md` 保持轻量：只做触发、路由、安全和回退。
- 详细能力下沉：按业务领域拆分到 `domains/*.md`。
- 场景流程模板化：放在 `recipes/*.md`。
- 参数和意图机器可读：放在 `schemas/*`。

## 分层关系（关键）

- **plugin = 执行层**：给 `opencli` 增加真实可执行命令（YAML/TS/JS adapter），例如 `opencli plugin install ...` 后得到新命令。
- **skill = 认知层**：告诉 Agent 何时调用哪些命令、如何补参数、何时确认风险、失败后如何降级。

两者不是替代关系，而是上下层关系：

1. plugin 决定“能不能做”
2. skill 决定“怎么用得对”

## 为什么按领域分组（而非 read/write）

命令量上来后，用户意图通常是“我要做内容运营/社区巡检/行情分析/开发诊断”，而不是“我要执行 read 操作”。

按领域组织有三个好处：

- 对齐用户表达：减少路由歧义
- 便于扩展：新平台只需挂到对应领域
- 便于权限控制：同领域统一风险策略

## 示例（OpenCLI 风格）

```bash
# 内容领域：抓取 B 站热榜
opencli bilibili hot --limit 20

# 社区领域：查看 HackerNews 热门
opencli hackernews top --limit 30

# 金融领域：查看雪球热股
opencli xueqiu hot --limit 20

# 开发工具领域：查看 GitHub issue
opencli gh issue list --repo owner/repo --limit 20
```

## 目录

- `SKILL.md`：路由入口（薄）
- `domains/`：领域能力说明
  - `content.md`
  - `community.md`
  - `finance.md`
  - `devtools.md`
- `recipes/`：场景化工作流
- `schemas/`
  - `intent-map.yaml`：意图映射
  - `args.schema.json`：统一参数结构
