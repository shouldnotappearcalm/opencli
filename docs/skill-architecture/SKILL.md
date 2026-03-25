---
name: opencli-domain-skill
description: OpenCLI 高命令量场景的按领域路由入口（content/community/finance/devtools）
---

# SKILL Router (Thin Entry)

## 何时使用

当用户需求属于以下任一领域时使用本 skill：

- content：内容选题、热榜收集、素材汇总、发布准备
- community：社区趋势、舆情观察、论坛动态
- finance：行情观察、股票热度、财务信息抓取
- devtools：GitHub/CLI 工具链查询与自动化辅助

## 何时不要使用

- 用户需要实现新的 adapter/plugin（应走 plugin 开发流程）
- 用户请求与 OpenCLI 能力无关（普通聊天、纯本地计算）
- 需要强交互网页自动化且命令不存在（先补 plugin）

## 能力边界

- 本 skill 负责：意图理解、领域路由、参数补全、风险控制。
- 本 skill 不负责：替代 plugin 的真实执行能力。
- 不臆造命令；无法确认时先 `opencli list` 或要求澄清平台/动作。

## 安全规则（必须遵守）

- 所有写操作（发帖、评论、点赞、关注、check-in、删除）必须二次确认。
- 支持 `dryRun=true` 时，默认先 dry-run。
- 涉及账号/资金/公开发布的动作，必须回显关键参数供用户确认。

确认模板：

> 即将执行写操作：`<command>`
> 目标平台：`<platform>`
> 影响对象：`<target>`
> 请输入“确认执行”继续。

## 失败回退

1. **命令不存在** → 建议领域内替代命令或切换平台。
2. **鉴权失败** → 提示登录/扩展连接状态（opencli doctor）。
3. **参数缺失** → 最少提问原则，仅追问必要字段。
4. **平台限流/异常** → 降低 `limit`、缩短时间窗口、稍后重试。
5. **写操作失败** → 返回失败原因 + 可重试命令（优先 dry-run）。

## 路由入口

- 领域细节：`domains/*.md`
- 场景流程：`recipes/*.md`
- 机器可读映射：`schemas/intent-map.yaml`
- 参数规范：`schemas/args.schema.json`
